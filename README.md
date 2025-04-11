# TE

Rafael de Morais Kataoka
- Criei a Chave e Clonei o repositorio fiz git pull apos o commit de vitorhugo e adicionei o algoritmo de subtração e divisão.

Rafael de Morais Kataoka
- Criei a Chave e Clonei o repositorio e adicionei o algoritmo de subtração e divisão.


Comandos de Vitor Hugo Cardozo de Abreu:

$ ssh-keygen -t rsa -b 4096 -C vitorhugocdz@edu.unifil.br
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/compuni/.ssh/id_rsa):
/c/Users/compuni/.ssh/id_rsa already exists.
Overwrite (y/n)?

compuni@Lab6m61 MINGW64 ~
$

compuni@Lab6m61 MINGW64 ~
$ ssh-keygen -t rsa -b 4096 -C vitorhugocdz@edu.unifil.br
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/compuni/.ssh/id_rsa):
/c/Users/compuni/.ssh/id_rsa already exists.
Overwrite (y/n)? y
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/compuni/.ssh/id_rsa
Your public key has been saved in /c/Users/compuni/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:VNYo0nz6codXgLohu3oKdWfJMOWGobAgB2zB72DIMCc vitorhugocdz@edu.unifil.br
The key's randomart image is:
+---[RSA 4096]----+
|*o+   .o. o+     |
|E*.o ..=+o+ o    |
|=+o . +.+=   .   |
|.+ .  .*+.    .  |
|. o . .oS+ . .   |
|   o ..oo + o    |
|  .    . o o     |
|   .  o          |
|    o+           |
+----[SHA256]-----+

compuni@Lab6m61 MINGW64 ~
$ eval "$(ssh-agent -s)"
Agent pid 1122

compuni@Lab6m61 MINGW64 ~
$ ssh-add ~/.ssh/id_rsa
Identity added: /c/Users/compuni/.ssh/id_rsa (vitorhugocdz@edu.unifil.br)

compuni@Lab6m61 MINGW64 ~
$ clip < ~/.ssh/id_rsa.pub

compuni@Lab6m61 MINGW64 ~
$ ssh -T git@github.com
Hi vitorcdz! You've successfully authenticated, but GitHub does not provide shell access.

compuni@Lab6m61 MINGW64 ~
$ git clone https://github.com/vitorcdz/TE.git
Cloning into 'TE'...
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 7 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (7/7), done.

compuni@Lab6m61 MINGW64 ~
$ cd TE

compuni@Lab6m61 MINGW64 ~/TE (main)
$ git checkout alteracoes
Switched to a new branch 'alteracoes'
branch 'alteracoes' set up to track 'origin/alteracoes'.

compuni@Lab6m61 MINGW64 ~/TE (alteracoes)
$ git add .

compuni@Lab6m61 MINGW64 ~/TE (alteracoes)
$ git commit -m AdicionarSomaeMultipicação
[alteracoes 0dee1a4] AdicionarSomaeMultipicação
 1 file changed, 15 insertions(+)

compuni@Lab6m61 MINGW64 ~/TE (alteracoes)
$ git push

Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 481 bytes | 240.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/vitorcdz/TE.git
   daa1970..0dee1a4  alteracoes -> alteracoes

compuni@Lab6m61 MINGW64 ~/TE (alteracoes)
$

compuni@Lab6m61 MINGW64 ~/TE (alteracoes)
$
