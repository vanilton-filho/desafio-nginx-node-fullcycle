# Desafio Full Cycle [Nginx, Node.js e MySQL]

Nesse desafio foi desenvolvido um proxy reverso utilizando o Nginx
para uma aplicação Node.js com o framework Express e o MySQL
como banco de dados.

O objetivo era fazer um proxy de modo que ao acessar localhost:8080 onde
está exposto o Nginx, seja redirecionado para a aplicação Node.js, e ao carregar
a página seja impresso "Full Cycle Rocks!", que seja inserido um nome de pessoa
no banco de dados e imprima também a lista desses nomes inseridos.

Utilizei a API [gerador-nomes](https://github.com/centraldedados/gerador-nomes) para gerar nomes
aleatórios a serem adicionados na base. Toda vez que acessar a página um novo
nome é adicionado e a lista é atualizada.

Foi adicionado o `nodemon` como servidor para trabalhar com o desenvolvimento de nossa app permitindo
que possamos ir alterando e salvando os nossos arquivos JavaScript, bastando dar o refresh na página
para ver o resultado.

Para testar utilize o seguinte comando:

`docker-compose up --build`
