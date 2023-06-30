# App Food

# Instalar as dependencias do projeto Node.js a partir do arquivo package.json

npm install

# Instalar o Yarn globalmente no sistema

npm install -g yarn

# Iniciar um conteiner Docker com uma instancia do MongoDB

docker run --name mongodb -d -p 27017:27017 mongo

# Iniciar o servidr de desenvlvimento do projeto

yarn dev

######

# Criando requisições GET e POST com INSOMNIA

Com o aplicativo instalado, devemos criar duas requisições, uma com nome List Categories com tipo GET e outra com nome Add Category com tipo POST.

Para criar, basta clicar no botão + e em HTTP request.

Feito isso, tanto no Add Category quanto no List Categories, devemos alterar o endereço das requisições, do lado do tipo (POS/GET) para o seguinte:

localhost:3000/categories

Na requisição POST no insomnia, podemos selecionar a aba Body, e no submódulo TEXT, selecionar a opção JSON. Dessa forma podemos escrever os parâmetros e seu conteúdo na parte "digitável" da página que será liberada. Podemos escrever conforme abaixo, onde usei o exemplo de um ícone de pizza.

{
    "name": "Pizza",
    
    "icon": "🍕"
}

