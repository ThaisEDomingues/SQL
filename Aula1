-- Aula1

-- cria o banco de dados
create database generation_brasil;
-- USE para usar o banco de dados
use generation_brasil;

-- criar uma tabela de cursos
create table cursos(
-- id_curso integer primary key auto_increment,
-- o comando acima é uma forma didatica de fazer um ID
id_curso varchar(36) default (uuid()) primary key,
-- (uuid()) gera uma chave unica aleatoria, sendo mais segura que auto_increment
titulo_curso varchar(255) not null,
turma_curso varchar(255) not null,
data_inicio_curso date not null
);

-- drop table NOME_DA_TABELA
-- ATENÇÂO se realizar o "drop" na tabela é 
-- apagado a tabela inteira e todos os seus registros 

-- para alterar as colunas da tabela
alter table cursos
-- "add column" comando para adicionar nova coluna
add column dataFim_curso date not null after turma_curso;


alter table cursos
-- "rename" renomeia a coluna
rename column data_inicio_curso to dataInicio_turma;

alter table cursos
-- "modify" altera a coluna selecionada inteira podendo mudar as regras como por exemplo varchar(255) para varchar(50)
modify column titulo_curso varchar(50) not null;

-- Populando Dados
insert into cursos (titulo_curso,turma_curso,dataInicio_turma,dataFim_curso) values
('analista de dados', 'gen02', '2026-03-30', '2026-06-28'),
('curso2', 'turma 2', '2026-02-02', '2026-03-03'),
('curso3', 'turma 3', '2026-05-05', '2026-06-06');

-- ver os dados
select * from cursos;
