# ARQUITETURA-DE-PROJETO-MVC-EXPRESS-WEBPACK
Repositório com modelo de arquitetura de projeto MVC com express + webpack

MVC:

MODEL -> base de dados

VIEW -> frontEnd

CONTROLLER -> funções/classes/tratamentos

ROUTER -> cria/aponta a rota(pagina) express e importa o controller


---

PASSO 1: criar estrutura mvc (src/controller, model e view);

PASSO 2: instalar express, nodemon, path e ejs no terminal;

PASSO 3: criar o server.js;

PASSO 4: criar o routes.js e as rotas (express.router()), exportar e importar controller;

PASSO 5: criar controller (específico para cada area do app), criar funções e importar o router;

PASSO 6: criar o index.ejs (bem parecido com HTML) dentro de views e todas as outras paginas;

PASSO 7: trocar o res.send para res.render na controller;

PASSO 8: criar pasta public (estáticos);

PASSO 9: criar pasta assets.



*res.send* = envia direto o html para a página
*res.render* = importa o html da view

# COMO FAZER O NODEMON IGNORAR PASTAS?

no package.json:
"scripts": {
    "start": nodemon server.js --ignore public
}

COMO RESOLVER VULNERABILILDADES DO NODE?

~npm audit fix

# COMO TESTAR ARQUIVO ESTÁTICO

conteúdo estático = logo, imagens, bundle, css, etc...

*como testar se conteúdo estático funciona:*
passo 1: cria um arquivo.txt;

passo 2: aponta caminho da pasta static no server;

passo 3: abre o navegador e põe /arquivo.txt.