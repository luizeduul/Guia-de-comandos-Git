<h1 align="center">
  <img alt="Git" src="https://ik.imagekit.io/8qmbx6p1dq/Assets/git_DHhJGSzaU.jpg" width="250px" />
</h1>

<p align="center">
 <img alt="License" src="https://img.shields.io/badge/license-MIT-brightgreen">
</p>

## Índice
- [O que é](#o-que-é-git)
- [Como utilizar](#como-utilizar)
- [Principais comandos](#principais-comandos)
- [Enviar ao github](#como-enviar-para-o-repositório-remoto)

### O que é git
<p>Git é um sistema open source de controle de versão de software. É o mais utilizado por toda a comunidade de programadores. Ele é bem fácil de ser aprendido e pode ser usado em qualquer tipo de projeto, de pequenos a grandes projetos.</p>

---
### Como utilizar

<p>Primeiramente é necessário fazer o download do git na sua máquina, para mais detalhes consulte o site do git abaixo.</p> 

[Site oficial do Git](https://git-scm.com/) 

<p>Tendo o software do git devidamente instalado, recomendo utilizar o Gitbash (linha de comando do git) para realizar as tarefas de controle de versão.</p>

---
### Principais comandos

<p><strong>git init</strong>: Esse comando vai inicializar o git em seu projeto</p>
<p><strong>git clone</strong> : Esse comando vai clonar um repositório na sua máquina local.</p>
<p><strong>git add .</strong> : Adiciona todos os arquivos para o git rastrear.</p>
<p><strong>git add nome_do_arquivo</strong> : Adiciona um arquivo ou pasta específica ao git.</p>
<p><strong>git commit -m</strong> : Realiza o commit com as alterações no repositório local. O -m é a mensagem que será adicionada ao commit para identificar mais facilmente as alterações feitas.</p><br/>

<p><strong>git status</strong> : Exibe o status dos arquivos no repositório local.</p>
<p><strong>git log</strong> :Devolve um historico de alterações que o repositorio sofreu ao longo do tempo.</p>
<br/>
<p><strong>git branch nome_da_branch</strong> : Cria uma nova ramificação para o repositorio, usado para criar novas funcionalidades de forma independente da branch principal</p>
<p><strong>git branch</strong> : Exibe a lista de branchs existentes.</p>
<p><strong>git checkout nome_da_branch></strong> : Muda para a branch escolhida.</p>
<p><strong>git checkout -b nome_da_branch</strong> : Cria uma branch e muda pra ela.</p>
<p><strong>git branch -D nome_da_branch</strong> : Deleta a branch.</p>
<br/>
<p><strong>git push</strong> : Serve para publicar as alterações num servidor remoto(intranet, github, etc)</p>
<p><strong>git pull</strong> : Serve para atualizar o repositório local com as alterações feitas no repositório remoto.</p>
<p><strong>git merge</strong> : Serve juntar as alterações de uma determinada branch com a branch merge, (merge) resoluções de conflitos qdo o git não consegue identificar quem fez as alterações de um determinado arquivo, 2 pessoas alterando o mesmo arquivo e não permite o push enquanto não arrumar manualmente o codigo.</p>
<br/>
<p><strong>git push origin nome_da_branch</strong> : Envia as alterações para o repositório remoto.</p>
<p><strong>git remote rm origin</strong> : Desvincula o repositório local com a origem do repositório remoto.</p>
<p><strong>git branch -D nome_da_branch</strong> : Deleta a branch.</p>
<p><strong>git push -u origin master</strong> : Ele informa que para cada branch que está atualizado ou que foi enviado com êxito, deve adicionar a referência de upstream (rastreamento)..</p>

-[git documentation](https://git-scm.com/docs) : Para mais comandos e informações, consulte a documentação completa do git.

---
### Como enviar para o repositório remoto

<p>Enviar o projeto para o repositório remoto é relativamente fácil.</p>
<p>A sequência básica de comandos é:</p>

```bash

    #1 Inicializar o repório local
    $ git init

    #2 Adicionar os arquivos do projeto
    $ git add project/

    #3 Verificar o status para saber se todos os arquivos desejados foram adicionados
    $ git status

    #4 Fazer o commit dos arquivos
    $ git commit -m"Commit example"

    #5 Adicionar a origin do repositório remoto (isso só deve ser feito na primeira vez, depois só fazer push)
    $ git remote add origin https://github.com/luizeduul/aula_git.git

    #6 Fazer o push para o repositório
    $ git push -u origin master

```

<p>Feito os comandos acima, se tudo ocorrer bem, seu projeto estará no Github</p>
<span>Obs. Após colocar o projeto no github, voce poderá pular o passo 1 e 5. No passo 6 deverá retirar o -u do comando apenas.</span>
<span>Nos comandos acima, se quiser enviar para uma branch remota diferente, basta substituir "master" pelo nome da branch desejada. Ex. $ git push origin branch1 . Este sifrão "$" é colocado automaticamente pelo Git Bash, então não é necessário escrever de novo.</span>
