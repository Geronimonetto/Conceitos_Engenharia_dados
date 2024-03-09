
- Não se trata apenas de um repositório de documentos!
- Sistemas de arquivos orientados a dados armazenam dados vivos que são usados para transição entre diferentes sistemas.
- Características do armazenamento de arquivos:
	- Versionamento - manter as versões diferentes dos arquios
	- Segurança - quem pode controlar os arquivos, ou do ponto de vista criptográfico.
	- Ciclo de vida - Requisito de acordo com o ciclo de tempo de vida do arquivo
- Características relacionados a "Big Data":
	- Particionamento - Do ponto de vista do Big data os arquivos tem um otimização de consulta quando estão particionados, são bastante utilizados atualmente.
	- Escalabilidade - aumento da capacidade
- Exemplos de armazenamento de arquivos:
	- S3
	- HDFS
	- Azure Blob Storage

## AWS S3
- Bucket funciona como uma pasta raiz
- Deve ter um nome único global
- A chave do arquivo tem o nome da bucket como início:
	- bucket/vendas.csv
	- bucket/pasta1/pasta2/vendas.csv
- É bastante útil e interessante quando olharmos partições
- Tags de objetos (Chaves para controle do ciclo de vida) - informando quando um arquivo tem informações sensíveis do cliente.
- Criação de Data Lake
- Formatos mais comuns para Eng de dados: CSV, JSON, Parquet, ORC

#### Particionamento do armazenamento de arquivos

- O particionamento de pastas por ano-mês-hora ajuda na otimização da consulta
	- s3://bucket//vendas/ano/mes/dia/hora/vendas.csv
- e também separar por produto
	- s3://bucket/vendas/1212/vendas.csv
- Você pode definir qual estratégia de particionamento você prefere
- O particionamento pode ser feito pelas próprias ferramentas do AWS Glue