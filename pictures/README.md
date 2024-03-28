SELECT count(*) FROM credito

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/f8acc616-f7f2-4a7b-8731-c00fd02d2956)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/0c6e62f6-4b19-4cff-8014-a7204450f20d)


Query: SELECT * FROM credito LIMIT 10;

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/54081c8e-a20d-4935-ab1d-b7723b0b23c6)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/963605cf-6257-401d-910f-7dc770bd83d9)

Query: DESCRIBE credito

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/d88d537e-53e8-42a3-8fb2-270768ba3cc5)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/88bd74b1-4716-419a-9f43-918788c9a0c8)

Query: SELECT DISTINCT escolaridade FROM credito

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/961a9e03-44a0-4fb5-8564-e333a2c16636)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/69efad02-787c-4b03-bd4f-d53f262eaef5)

Query: SELECT DISTINCT estado_civil FROM credito

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/cc2fab6e-5412-4415-a503-0218dd14b864)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/092da1ea-5983-4c00-8672-2f2606cc9581)

Query: SELECT DISTINCT salario_anual FROM credito

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/75c3bc7e-5653-4305-8d30-f0f2ce6bb3cd)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/4e7907ea-053c-4329-a070-0e439ff920b4)

Query: SELECT DISTINCT tipo_cartao FROM credito

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/972615ca-a37b-4067-9f86-5f3189957ed1)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/8583c01d-7b17-4f6a-9ea0-43d6a1497447)

Query: select count(*), salario_anual from credito group by salario_anual

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/61ee0090-ea6d-47b6-b5c9-f3187df9446a)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/a0079e31-3ab9-47e5-bd4d-a916c884f9e4)

Query: select count(*), sexo from credito group by sexo

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/51fec78a-37b7-41af-b9c0-e22aaab23d77)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/ecdb3b23-8152-4455-a443-c964f4e58b50)



$$ Grafico pizza F/M
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/97b7e776-0972-4de3-854a-43102520f5d3)


Query: select avg(idade) as media_idade, min(idade) as min_idade, max(idade) as max_idade, sexo from credito group by sexo

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/b3625d94-3e5f-48e1-bdec-b4a0839b273c)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/b5f9621a-52b7-450a-8215-ebc0a669f2b0)

Query: select min(valor_transacoes_12m) as transacao_minima, max(valor_transacoes_12m) as transacao_minima from credito

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/721ed4f4-bc9e-485d-b961-5b6e3f88b62a)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/0100c727-29c5-4ed7-a452-9980fe8249ab)

Query: select max(limite_credito) as limite_credito, escolaridade, tipo_cartao, sexo from credito where escolaridade != 'na' and tipo_cartao != 'na' group by escolaridade, tipo_cartao, sexo order by limite_credito desc limit 10

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/8d950774-d8ad-4064-a3c1-4d4a8919140b)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/e0cf5d89-7676-415d-bb50-64481c18a33a)


Query: select max(limite_credito) as limite_credito, escolaridade, tipo_cartao, sexo from credito where escolaridade != 'na' and tipo_cartao != 'na' group by escolaridade, tipo_cartao, sexo order by limite_credito asc limit 10;

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/e2cca9bc-e97b-4a69-8639-5401b3ff9a03)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/223bc4de-cc8f-4585-99eb-78467a141ff9)

 select max(valor_transacoes_12m) as maior_valor_gasto, avg(valor_transacoes_12m) as media_valor_gasto, min(valor_transacoes_12m) as min_valor_gasto, sexo from credito group by sexo

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/c63fec6a-4976-4e2d-b892-4f9dc6af922a)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/0b8e5b4a-fd43-4b1b-b1e2-dfce6cbb676b)

Query: select avg(qtd_produtos) as qts_produtos, avg(valor_transacoes_12m) as media_valor_transacoes, avg(limite_credito) as media_limite, sexo, salario_anual from credito where salario_anual != 'na' group by sexo, salario_anual order by avg(valor_transacoes_12m) desc

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/7372c28c-fe49-4b2c-a47c-3a2f0061db09)
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/3dcda4c5-d935-47e8-b9dc-1b2a0f39323f)


![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/8c71202c-49f4-4d69-a50a-93ad10b98035)



![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/6a01b517-2c5b-4a78-ae85-0b19a2a271d8)


-------



![projeto telegram 2](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/4c08838a-44b3-4bde-8c60-d2d0f27637d4)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/b36995d2-4ac9-4917-9952-47f68ca34f16)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/c2e3d6dd-2ae5-4cb1-9010-d7d3806f261e)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/1cceab3d-20d2-4498-ae3b-cd1c053867b9)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/a58839da-25fe-4cb7-abdb-349e04b6945e)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/5c921b22-1fbb-4639-99e5-d667b001e813)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/901c03b9-ed04-4f0f-a1c5-33aae38fca46)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/c00cbfa9-a7fa-447a-b165-9316fe6e0ecf)






![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/3c7fc8a8-6141-428d-80db-c0aca073d32d)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/ddd7fed7-a0e5-4664-a9ef-3ace126705e3)


![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/0ba3b248-aace-4b7d-9492-2c80cea31729)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/42df0e6f-e817-452a-b158-3707b7c71c22)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/4f644df6-f2fd-4fe7-a80e-ab173dce61a0)


![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/5198f7d5-35f3-4ee7-b69d-f58da25a80cd)

exercicio 2

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/ae5ebdfb-df43-456b-9e57-0c0842e96923)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/27204a5c-e372-4e4a-a73d-03c962e86c0c)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/fb74dd26-ec3e-45f2-8cc7-f1f086a3c6f3)


![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/7163d9cd-a4fb-4576-8a29-773c3e298fa6)


![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/693b2cf0-2cc9-4e76-bd27-9b16e16c08a9)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/7411a8ea-9f14-482f-a3f7-683ee93b2ad1)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/e29d84f2-54ac-4669-9a9a-45e67809cdf6)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/b8dd5f38-eb0d-4786-a126-7818a6254928)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/fd4776fa-c474-4916-be77-818729c928e8)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/fdbae055-a8c1-4601-9136-1479e1fe1146)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/1b05b39a-4197-4999-ac48-fb9811f89c89)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/fbc0ade7-55cf-4eb0-9f70-29626fa6b8bb)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/bd5076a7-2101-42b4-a637-0ecc1b3a1076)


continuação projeto

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/5d34995a-d34a-4c0c-ae1c-5e45fd108227)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/4828e664-8f94-4598-8ec7-351dd0aed2e0)


![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/a4b781cb-1e79-4932-90b7-c0de631a3772)


![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/953f410a-e121-44d8-b81c-60565fe1b44b)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/9dde8c2f-2fed-4bd4-b3bf-048d0bd90a94)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/912ddfcf-a7c9-44e1-94c5-7a93f628a834)



![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/6510e6b1-0569-40d0-8ae8-4cb57c676d5e)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/693fce60-6c2e-4bd2-94a6-e7222c3c42d5)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/c339c77d-4596-426e-a75a-30d947e786ac)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/7233263a-9359-45d0-bca8-53075ffb33b0)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/f333fffd-2045-40bd-bcbf-fdd170d98af2)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/dbc9a889-a66b-4f66-9f7a-c755d59354fc)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/0ba47cc4-0c66-4f13-93c2-1719e641f953)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/c3c91e38-a9bb-41f9-b51a-8eaae097980f)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/12695124-5a97-456a-a8c4-d707b2ab7b8b)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/d64edb89-0b32-49a5-8286-6c166ca6e364)


![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/1058a2ad-9971-4ee7-ae56-e0e36dac1081)

![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/8360d95e-5359-40a0-be24-fdc1ad6b422c)
Dashboard
![image](https://github.com/JosueMorfim/Analise_Credito_SQL/assets/141301164/a4f39298-3955-4aea-9b27-0d50e92128ea)








