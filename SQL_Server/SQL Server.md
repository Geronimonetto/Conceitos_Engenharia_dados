# **SQL Server**

Pode-se criar os 2 tipos de bancos de dados no SQL Server, tanto gerencial quanto transacional.

**Banco de dados gerencial** - Os processos de ETL e ELT são criadas várias linhas no DW, quando refazemos o processo de ETL não é preciso salvar os Logs, por que executando o ETL os dados são recuperados rapidamente.  
  - Backups do tipo full

**Banco de dados transacional** - é o banco de dados operacional, que controlam as atividades do dia a dia da empresa.  
  - Podemos fazer backups ativando os logs - porém consome muito espaço  
  - Pegar os históricos

```sql  
CREATE DATABASE DW_ATACADEZ;  -- comando para criar DATABASE  
ALTER DATABASE [DW_ATACADEZ] SET RECOVERY SIMPLE;  -- retirando o salvamento de logs

```

O Código acima faz com que o DW não salve os logs de transações.