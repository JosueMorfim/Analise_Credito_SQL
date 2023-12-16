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



