Para rodar essa aplicação localmente, primeiro é necessário ter instalado o arquivo “todo_list”, após a instalação do arquivo é preciso também extrair o arquivo. Depois é preciso instalar o WAMP ou XAMPP. Caso esteja utilizando o WAMP, entre nos arquivos do WAMP e coloque a pasta “todo_list” dentro da pasta “www”. Mas caso o XAMPP esteja sendo utilizado, entre nos arquivos do XAMPP e coloque a pasta “todo_list” dentro do arquivo “htdocs”. Após ter colocado a pasta do projeto no WAMP ou no XAMPP agora é necessário que seja aberto o phpMyAdmin. Após abrir o phpMyAdmin, coloque o usuário “root” e senha em branco para que o projeto possa funcionar sem erros. Depois de ter logado no phpMyAdmin, crie um banco de dados chamado “todo_list” após isso, clique no banco de dados “todo_list” e depois clique na opção “SQL”. Nesta opção será criada a tabela onde serão armazenados os dados, o código para a criação da tabela é:

CREATE TABLE tasks (
id INT AUTO_INCREMENT PRIMARY KEY,
title VARCHAR(255),
description TEXT,
created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP ON UPDATE
CURRENT_TIMESTAMP
);

Para executar este código é só clicar no botão “Execute” na parte inferior da tela.
Após a tabela ter sido criada e o WAMP ou XAMPP estiver aberto, digite “localhost/todo_list” com isso você já vai estar rodando a aplicação localmente.
