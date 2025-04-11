# TE

Rafael de Morais Kataoka
- Criei a Chave e Clonei o repositorio fiz git pull apos o commit de vitorhugo e adicionei o algoritmo de subtração e divisão.


## Comandos utilizados

rafae@AnonymousVS MINGW64 ~
$ rm -f ~/.ssh/id_rsa*

rafae@AnonymousVS MINGW64 ~
$ ssh-keygen -t rsa -b 4096 -C rafaelrmk@edu.unifil.br
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/rafae/.ssh/id_rsa):
Enter passphrase for "/c/Users/rafae/.ssh/id_rsa" (empty for no pas
Enter same passphrase again:
Your identification has been saved in /c/Users/rafae/.ssh/id_rsa
Your public key has been saved in /c/Users/rafae/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:D4xL53XLdwqF6aSkFqTr1DX4q3DxMI2m1s+k1qtQfqk rafaelrmk@edu.un
The key's randomart image is:
+---[RSA 4096]----+
|                 |
|                 |
|        .        |
|       = +   o   |
|      + S * = .  |
|     . % # O o   |
|      O O.O = . .|
|     + =.B.. o o |
|      ..Eo=.  .  |
+----[SHA256]-----+

rafae@AnonymousVS MINGW64 ~
$ eval "$(ssh-agent -s)"
Agent pid 1245

rafae@AnonymousVS MINGW64 ~
$ ssh-add ~/.ssh/id_rsa
Identity added: /c/Users/rafae/.ssh/id_rsa (rafaelrmk@edu.unifil.br

rafae@AnonymousVS MINGW64 ~
$ clip < ~/.ssh/id_rsa.pub

rafae@AnonymousVS MINGW64 ~
$ ssh -T git@github.com
Hi KataokaRmk! You've successfully authenticated, but GitHub does nell access.

rafae@AnonymousVS MINGW64 ~
$ git clone git@github.com:vitorcdz/TE.git
Cloning into 'TE'...
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 7 (delta 0), reused 0 (delta 0), pack-reused 0 (from
Receiving objects: 100% (7/7), done.

rafae@AnonymousVS MINGW64 ~
$ cd git@github.com:vitorcdz/TE.git
bash: cd: git@github.com:vitorcdz/TE.git: No such file or directory

rafae@AnonymousVS MINGW64 ~
$ cd TE

rafae@AnonymousVS MINGW64 ~/TE (main)
$ git checkout alteracoes
branch 'alteracoes' set up to track 'origin/alteracoes'.
Switched to a new branch 'alteracoes'

rafae@AnonymousVS MINGW64 ~/TE (alteracoes)
$ git add .

rafae@AnonymousVS MINGW64 ~/TE (alteracoes)
$ git commit -m adicioneisubtraçãoedivisão
[alteracoes 59281b2] adicioneisubtraçãoedivisão
 2 files changed, 27 insertions(+), 1 deletion(-)

rafae@AnonymousVS MINGW64 ~/TE (alteracoes)
$ git push
To github.com:vitorcdz/TE.git
 ! [rejected]        alteracoes -> alteracoes (fetch first)
error: failed to push some refs to 'github.com:vitorcdz/TE.git'
hint: Updates were rejected because the remote contains work that y
hint: have locally. This is usually caused by another repository pu
hint: the same ref. If you want to integrate the remote changes, us
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for d

rafae@AnonymousVS MINGW64 ~/TE (alteracoes)
$ git push
To github.com:vitorcdz/TE.git
 ! [rejected]        alteracoes -> alteracoes (fetch first)
error: failed to push some refs to 'github.com:vitorcdz/TE.git'
hint: Updates were rejected because the remote contains work that y
hint: have locally. This is usually caused by another repository pu
hint: the same ref. If you want to integrate the remote changes, us
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for d

rafae@AnonymousVS MINGW64 ~/TE (alteracoes)
$ git pull
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 3 (delta 0), pack-reused 0 (from
Unpacking objects: 100% (4/4), 1.33 KiB | 194.00 KiB/s, done.
From github.com:vitorcdz/TE
   daa1970..0dee1a4  alteracoes -> origin/alteracoes
   79b959a..bb4370d  main       -> origin/main
Auto-merging algoritmo.por
CONFLICT (content): Merge conflict in algoritmo.por
Automatic merge failed; fix conflicts and then commit the result.

rafae@AnonymousVS MINGW64 ~/TE (alteracoes|MERGING)
$ ^C

rafae@AnonymousVS MINGW64 ~/TE (alteracoes|MERGING)
$ git reset --soft
fatal: Cannot do a soft reset in the middle of a merge.

rafae@AnonymousVS MINGW64 ~/TE (alteracoes|MERGING)
$ git push
To github.com:vitorcdz/TE.git
 ! [rejected]        alteracoes -> alteracoes (non-fast-forward)
error: failed to push some refs to 'github.com:vitorcdz/TE.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

rafae@AnonymousVS MINGW64 ~/TE (alteracoes|MERGING)
$ git add .

rafae@AnonymousVS MINGW64 ~/TE (alteracoes|MERGING)
$ git commit -m "merge"
[alteracoes 6b37536] merge

rafae@AnonymousVS MINGW64 ~/TE (alteracoes)
$ git push
Enumerating objects: 13, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 12 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 926 bytes | 926.00 KiB/s, done.
Total 7 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To github.com:vitorcdz/TE.git
   0dee1a4..6b37536  alteracoes -> alteracoes

### Comandos de Fulano

### Comandos de Ciclana

### Comandos de beltrano
