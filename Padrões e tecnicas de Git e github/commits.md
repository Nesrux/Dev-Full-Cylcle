# Padronização de commits
Existe uma especifição de commits que servem para manter a organização dos commits em um projeto, seja ele open-source ou não.
Eles seguem a especificação feita no projeto do Angular, que você pode ler na integra clicando <a hreaf ="https://www.conventionalcommits.org/pt-br/v1.0.0/">aqui<a/>


## Mas como Trabalhar com essa especificação ?
Existem varias formas de se trabalhar com ela, utilizando de plugins, extensoes ou até projetos feitos no docker, aqui iremos abordar algumas das alternativas.

### Convetional commits
Uma extensão feita para o VSCODE, ele é feita para facilitar o processo de escrita de commits, é muito simples a instalação, é só ir na loja de extensões do vscode e digitar, convetinal commits, e vai aparecer algumas extensões que fazem coisas parecidas, só escolher a que mais te agrada e utilizar!

### Commitzen
Mas e se eu não estiver usando o Vscode, existe outra alternativa ?
Com toda a certeza, uma boa alternativa é o Commitzen, ele é roda diretamente em seu terminal, seja ele Bash, Shell ou Powershel, mas para baixa-lo é necessario utizar o NPM para instalar ele.

primeiro verificamos se o NPM ja esta instalado em seu computador digitando o comando no terminal 

``npm -v``
se não der nenhum erro e aparecer a versão em seu terminal, quer dizer que o npm ja esta instalado.
Agora é só instalar co commitzen em seu computador utilizando o comando
``npm install commitizen -g``


``
npx commitizen init cz-conventional-changelog --save-dev --save-exact
``

precisa de um arquivo de gitignore, para nao pushar o nodemodules



rodar o commitzar`
serve para ser utilizado em CI (continus integrarion)
  docker run --rm --name="commitsar" -w /src -v "$(pwd)":/src aevea/commitsar commitsar .