### Principais comandos Git

## Iniciar repositório

* git init

## Verificar estado dos arquivos/diretórios

* git status

### Adicionar arquivo/diretório (staged area)
## Adicionar um arquivo em específico

* git add meu_arquivo.txt

## Adicionar um diretório em específico

* git add meu_diretorio

## Adicionar todos os arquivos/diretórios

* git add .

## Adicionar um arquivo que esta listado no .gitignore (geral ou do repositório)

* git add -f arquivo_no_gitignore.txt

## Comitar arquivo/diretório

* git commit meu_arquivo.txt

## Comitar vários arquivos

* git commit meu_arquivo.txt meu_outro_arquivo.txt

## Comitar informando mensagem

* git commit meuarquivo.txt -m "minha mensagem de commit"

## Remover arquivo/diretório

* git rm meu_arquivo.txt

## Remover diretório

* git rm -r diretorio

## Visualizar histórico

* git log

## Exibir histórico com diff das duas últimas alterações

* git log -p -2

## Exibir resumo do histórico (hash completa, autor, data, comentário e qtde de alterações (+/-))

* git log --stat

## Exibir informações resumidas em uma linha (hash completa e comentário)

* git log --pretty=oneline

## Exibir histório de um determinado autor

* git log --author=usuario

## Exibir revisão e autor da última modificação de uma bloco de linhas

* git blame -L 12,22 meu_arquivo.txt 

### Desfazendo alteração local (working directory)

## Este comando deve ser utilizando enquanto o arquivo não foi adicionado na staged area.

* git checkout -- meu_arquivo.txt

## Desfazendo alteração local (staging area)
## Este comando deve ser utilizando quando o arquivo já foi adicionado na staged area.

* git reset HEAD meu_arquivo.txt