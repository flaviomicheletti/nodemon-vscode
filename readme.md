# Debugando JavaScript no VSCode com Nodemon

https://nodemon.io/

Criei uma aplicaçõa conforme [express-application-generator](https://github.com/flaviomicheletti/express-application-generator/tree/master)

Instalei as dependências

    npm i

Instalei também...

    npm install http-errors
    npm install -save-dev nodemon


### Iniciando o processo

Primeiro, inicie a aplicação.

    npm run debug

Que, em nosso caso, é equivalente a `nodemon --inspect ./bin/www`.

![nodemon-npm-run-debug](https://user-images.githubusercontent.com/1257048/86028749-a93be180-ba08-11ea-849c-ad7a76c75045.jpg)

Se você quiser, pode testar a aplicação http://localhost:3000/.

Agora vá para a visão de Debug pressionando `F5`.

Por enquanto, a única configuração que temos é a `Node + Nodemon`.

Selecione o processo que contenha a flag `--inspect`.

![nodemon-vscode-debug](https://user-images.githubusercontent.com/1257048/86028720-a214d380-ba08-11ea-9f49-97ae969ddd62.png)


### A mágica

Agora coloque um break point, por exemplo, no arquivo __user.js__ linha 06.

Acesse novamente a aplicação  http://localhost:3000/ e voialá.


### Ajudou muito...

https://github.com/microsoft/vscode-recipes/tree/master/nodemon