# Desnormalizando-dados-com-Power-BI

## Objetivo

**O objetivo é importar o modelo normalizado e desnormalizá-lo, criando um star schema com a tabela de fatos e a tabela de dimensão.**

![1](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/d06760d8-ee02-454a-9556-0cfa04426ab3)

1. Ingestão e analise dos dados

![2](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/672a24ba-03d3-4fb3-b71e-4a83fbc361e6)

* Substituir valores nulos (Null) por não se aplica (NA)
* Coluna Cor

![3](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/9bcd02b6-4ab1-407a-bbb4-ac2109dd820d)

* Coluna Tamanho

![4](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/f1d00eda-3095-4661-9dba-ab5d1f410a86)

* Criando copias de referência a partir da tabela base

![5](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/353d2d80-258b-4cb2-a7cc-eb49c5dda39b)

* Renomeando as referências e criando grupo para organizar

![6](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/b97215c5-30b3-4e12-9024-86aca4bbd716)

2. Eliminando colunas

* O objetivo dessa etapa é remover todas as colunas deixando somente a coluna com o nome da tabela.
* Tabela categoria
  
![7](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/5a278cf1-dd20-40e8-a89d-3d0690b2349d)

segue esse parão para todas as tabelas, tirando a tabela fato

3. Eliminando registros duplicados

* ultilizando remover duplicados na tabela categoria e nas demais.

![8](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/8220be4d-c043-4872-a485-946a74f4b8c3)

4. Adicionando chave artificial (SK) Surrogate key

* adicionando coluna índice e renomenado para ID_Categoria, segue o mesmo padrão para as outras tabelas.

![9](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/a562cf05-18f7-4a0b-85ba-957a354d6c75)

5. Combinando/Mesclando os dados da tabela

* Aqui nessa etapa irei ultilizar a opção mesclar consultas na tabela fato para fazer os Joins.

![10](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/1cd77b7b-ea97-4602-aa01-eabfa5420053)

* ID_Categoria na tabela Fato. Segue o mesmo padrão para as outras tabelas

![11](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/a8ac6606-2e83-40bf-bf5f-b9785e029a08) 

6. Eliminando colunas redundantes

* com a introdução das colunas IDs é necessário remover as colunas redundantes
  
![desnormalizando dados power bi](https://github.com/JulioMancini/Desnormalizando-dados-com-Power-BI/assets/145502330/dc1d55a2-507a-41c2-9168-1f6f9808bebe)

7. Relacionamento entre fato e dimenção (xibição de Modelo)




