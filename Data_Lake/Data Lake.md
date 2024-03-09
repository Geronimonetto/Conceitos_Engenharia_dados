
Os data lakes como o próprio nome diz é onde uma empresa armazena seus dados para futuras análises.

- Exemplo de data Lake - S3 (AWS)

Quando falamos de Data Lake estamos falando também de várias fontes de dados centralizadas em um ambiente apenas, ou seja, existem vários bancos de dados, ou fontes de dados de estruturas diferentes que estão centralizadas em apenas 1 local de armazenamento, facilitando um pouco o entendimento de como estão organizados os dados.
Normalmente os data lakes sofrem apenas alterações de inclusão e consultas, não é recomendado operação de exclusão ou atualização, o modelo dos dados do data lake é de modelo dimensional, essa forma é melhor por que é otimizada, mantem o histórico e fornecer informação para tomada de decisão.

Cada departamento dentro de uma empresa é recomendado que exista o seu próprio data mart (data lake por departamento).

Exemplo:
	- Produção
	- Vendas

Data WareHouse é o conjunto de Data Marts, reúne todos os dados de apoio a decisão da organização.

Diferença de Data Mart
- Local - é específico para um determinado departamento
- Corporativo -  é usado para atender a demanda da empresa

OLAP 

Sistemas analíticos ou On-line Analytical Processing é a capacidade para manipular e analisar um grande volume de dados sob múltiplas perpesctivas, ou seja, você pode analisar informaçõe sobre diversas perspectivas.

Exemplo:
	- Vendedor x 
	- qual empresa ele vendeu?
	- qual lugar ele mais vendeu?
	- qual data ele mais vendeu?

As informações geralmente estão modeladas de forma dimensional

Banco de dados operacional não mantém histórico das informações












