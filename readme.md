Projeto automação WEB com Cypress - Nível basíco
Projeto de automação web com Cypress, com ele você irá conseguir escrever seus primeiros casos de testes com uma ferramenta poderosa cheia de recursos que facilitam a sua vida.

Pré requisitos para utilizar o projeto
SO
macOS 10.9 e superior (Intel ou Apple Silicon 64-bit (x64 ou arm64))
Linux Ubuntu 20.04 e superior, Fedora 21 e Debian 8 (x86_64 ou Arm 64 bits (x64 ou arm64))
Windows 10 e superior (apenas 64 bits)
Hardware
Mínimo de 2 CPUs para rodar o Cypress
1 CPU adicional se a gravação de vídeo estiver ativada
1 CPU adicional por processo executado fora do Cypress, como:
Servidor de aplicativos (frontend)
Servidor de aplicativos (back-end)
Banco de dados de aplicativos
Qualquer infraestrutura adicional (Redis, Kafka, etc.)
Memória
Mínimo de 4 GB, 8 GB + para execuções de teste mais longos.
NodeJS
Node.js 18.x
Node.js 20.x ou superior
IDE
VSCODE
Qualquer outra de sua preferência
Links de instalação
NodeJs - https://nodejs.org/en/download
VSCODE - https://code.visualstudio.com/download
Documentos de referência
Cypress:
https://www.cypress.io/
https://example.cypress.io/commands/actions
https://docs.cypress.io/guides/core-concepts/writing-and-organizing-tests#Folder-Structure
Configurando ambiente para começar a usar o Cypress
Agora iremos configurar o ambiente para iniciarmos nosso projeto com o Cypress. Para isso é necessário realizar o download da IDE do VSCODE

01 Instalação inicial
Faça o download o NodeJS e instale a versão compatível com seu Sistema Operacional;
Faça o download e instale o VSCODE ou outra IDE de sua preferência;
02 Instale o Cypress
npm install cypress --save-dev
03 Observação
Está configurado no package.json, um bloco de script para executar o cypress

"scripts": {
    "cypress:open": "cypress open"
  }
A sintaxe "cypress:open" determina como será executado o cypress, recebendo a instrução padrão "cypress open"

04 Executando o cypress
   npm run cypress:open
Pronto agora é só criar seus cenários de testes e aproveitar o melhor da ferramenta.

** Instalação do Cypress **
npm install cypress --saved-dev

** Rodando Cypress **
npx cypress open  - abre o cypress studio - 
npx cypress run - abre em modo headless

** configurando palavra de execução para cypress open no "scripts" **
<pre>
{
  "dependencies": {
    "cypress": "^13.10.0"
  },
  "scripts":{
    "test": "npx cypress open", // roda interface do cypress
    "test2": "npx cypress run"  // roda em modo headless
  }
}
</pre>

