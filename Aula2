create database solar;
use solar;

SELECT * FROM dados_solar;
-- para colunas nomeadas com nome composto, é necessário utilizar
-- crase `` para realizar a leitura

-- "SHOW Tables" mostra todas as tabelas no banco de dados
-- selecionado anteriormente
SHOW Tables;

select Name, `kW AC`, address from dados_solar
order by name asc;
-- "order by" comando ordena os dados da coluna selecionada anteriormente
-- "asc" -> 0 a 9 ou "a" a "z"
-- "desc" -> 9 a 0 ou "z" a "a"

-- "count()" realiza a contagem de itens da coluna que está entre ()
select count(distinct `kW AC`) from dados_solar;
-- "distinct" realiza a contagem retirando todas as duplicadas
