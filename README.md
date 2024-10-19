# 📈📉📊 Estatística Criminal do Feminicídio nas Unidades da Federação

[![pptx](/Capa_pptx.png)](https://docs.google.com/presentation/d/1RHGsovdnWhP2myDpJVKSPxXjwzhzCGcH/edit?usp=drive_link&ouid=103014318842924902559&rtpof=true&sd=true)

## 📚 Descrição da Atividade

Projeto Final semana 17/18.

**Objetivo:** Esta análise tem como objetivo demonstrar a evolução do crime de feminicídio por estado nos anos de 2020 a 2024. 


O feminicídio é definido como o assassinato de uma mulher em razão de seu gênero, frequentemente associado à violência doméstica, discriminação ou desigualdade de gênero. 
Além de traçar o crescimento desse crime ao longo dos anos, a análise também busca compará-lo com o número de homicídios femininos ocorridos nos estados e verificar a 
porcentagem de feminicídios em relação ao total de homicídios femininos. Com isso, pretende-se evidenciar a 
gravidade e o impacto específico da violência de gênero no contexto dos crimes contra a vida.

  ### 📚 Descrição da Base:

A escolha do tema e das bases de dados foi motivada pelo interesse em compreender quais fatores podem impactar diretamente o aumento ou a redução dos casos de feminicídio no Brasil.

Bases tratadas na aula da semana 17 [Feminicídios](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/database-Feminicidio.csv) 
e [Homicídios do sexo Feminino](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/homicidios_femininos.csv) disponiveis neste repositório.

Após tratamento minha base de dados ficou assim:
A base final de dados [Feminicídio Por Estado](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/feminicidio.csv) é composta por 56 colunas:

| INDICE  | NOME DAS COLUNAS | CONTEUDO |
| ----- | --- | :---: |
|  0  |  estado  |  (26 Estados mais o Distrito Federal)  |
|  1  |  siglas  |  (Silas dos 26 Estados mais Distrito Federal)  |
|  2  |  regiao  |  (Regioes: Norte, Nordeste, Sul, Sudeste, Centro_Oeste)  |
|  3  |  total_municipos_por_estado(IBGE)  |  (Quantidade de Municipios por Estado)  |
|  4  |  renda_per_capita(IBGE)  |  (Renda Feminina Per Capta de cada Estado)  |
|  5  |  idh(IBGE)  |  (Taxa de IDH de casa Estado)  |
|  6  |  taxa_desemprego_feminino  |  (Taxa de desemprego Feminino, segundo IBGE)  |
|  7  |  delegacias_especializadas_de_atendimento_a_mulher  |  (Quantidade de Delegacias Especializadas por Estado)  |
|  8  |  feminicidio_tentado_2024(LESFEM)  |  (Quantidade de Feminicídio TENTADO no ano de 2024 por Estado)  |
|  9  |  feminicidio_consumado_2024(LESFEM)  |  (Quantidade de Feminicídio CONSUMADO no ano de 2024 por Estado)  |
|  10  |  ano_2024  |  (Coluna do Ano de 2024)  |
|  11  |  feminicidio_tentado_2023(FBSP)  |  (Quantidade de Feminicídio TENTADO no ano de 2023 por Estado)  | 
|  12  |  feminicidio_consumado_2023(FBSP)  |  (Quantidade de Feminicídio CONSUMADO no ano de 2023 por Estado)  |
|  13  |  ano_2023  |  (Coluna do Ano de 2023)  | 
|  14  |  feminicidio_tentado_2022(FBSP)  |  (Quantidade de Feminicídio TENTADO no ano de 2022 por Estado)  |
|  15  |  feminicidio_consumado_2022(FBSP)  |  (Quantidade de Feminicídio CONSUMADO no ano de 2022 por Estado)  |
|  16  |  ano_2022  |  (Coluna do Ano de 2022)  |
|  17  |  feminicidio_tentado_2021(FBSP)  |  (Quantidade de Feminicídio TENTADO no ano de 2021 por Estado)  |
|  18  |  feminicidio_consumado_2021(FBSP)  |  (Quantidade de Feminicídio CONSUMADO no ano de 2021 por Estado)  |
|  19  |  ano_2021  |  (Coluna do Ano de 2021)  |
|  20  |  Feminicidio Tentado  |  (Quantidade de Feminicídio TENTADO no ano de 2020 por Estado)  | 
|  21  |  Feminicidio Consumado  |  (Quantidade de Feminicídio CONSUMADO no ano de 2020 por Estado)  |
|  22  |  ano_2020  |  (Coluna do Ano de 2020)  |
|  23  |  indicador_conferencia_politicas_para_mulheres  |  (FRASE = 'Conferências nos últimos quatro anos sobre política para mulheres')  |
|  24  |  %_total_numero_municipios_conferencia_politicas_para_mulheres  |  (Porcentagem numerica em relação ao total de municípios que confirmam aplicar esta política pública)  |
|  25  |  numero_municipios_conferencia_politicas_para_mulheres  |  (Quantidade numerica de municípios que confirmam aplicar esta política pública)  |           
|  26  |  indicador_protecao_vitimas_violencia  |  (FRASE = 'Proteção de mulheres vítimas de violência doméstica')  |                            
|  27  |  %_total_numero_municipios_protecao_vitimas_violencia  |  (Porcentagem numerica em relação ao total de municípios que confirmam aplicar esta política pública)  |           
|  28  |  numero_municipios_protecao_vitimas_violencia  |  (Quantidade numerica de municípios que confirmam aplicar esta política pública)  |                   
|  29  |  indicador_lei_especifica_violencia  |  (FRASE = 'Lei Específica sobre Enfrentamento à violência contra a mulher')  |                              
|  30  |  %_total_numero_municipios_lei_especifica_violencia  |  (Porcentagem numerica em relação ao total de municípios que confirmam aplicar esta política pública)  |             
|  31  |  numero_municipios_lei_especifica_violencia  |  (Quantidade numerica de municípios que confirmam aplicar esta política pública)  |                       
|  32  |  indicador_prog_específicas_para_mulheres  |  (FRASE = 'Programas e ações específicas para mulheres')  |                        
|  33  |  %_total_numero_municipios_prog_específicas_para_mulheres  |  (Porcentagem numerica em relação ao total de municípios que confirmam aplicar esta política pública)  |       
|  34  |  numero_municipios_prog_específicas_para_mulheres  |  (Quantidade numerica de municípios que confirmam aplicar esta política pública)  |               
|  35  |  indicador_acoes_PM  |  (FRASE = 'Ações de Prevenção da Polícia Militar quanto ao Enfrentamento à Violência doméstica e de gênero')  |                                             
|  36  |  acoes_junto_a_PM  |  (SIM ou NÃO para o estado que aplica ou não esta política pública)  |                                                
|  37  |  tentativa_2020  |  (Quantidade de Homicídio Feminino TENTADO no ano de 2020 por Estado)  |                                              
|  38  |  consumado_2020  |  (Quantidade de Homicídio Feminino CONSUMADO no ano de 2020 por Estado)  |   
|  39  |  tentativa_2021  |  (Quantidade de Homicídio Feminino TENTADO no ano de 2021 por Estado)  |                                                   
|  40  |  consumado_2021  |  (Quantidade de Homicídio Feminino CONSUMADO no ano de 2021 por Estado)  |                                                  
|  41  |  tentativa_2022  |  (Quantidade de Homicídio Feminino TENTADO no ano de 2022 por Estado)  |                                                
|  42  |  consumado_2022  |  (Quantidade de Homicídio Feminino CONSUMADO no ano de 2022 por Estado)  |                                                  
|  43  |  tentativa_2023  |  (Quantidade de Homicídio Feminino TENTADO no ano de 2023 por Estado)  |                                                 
|  44  |  consumado_2023  |  (Quantidade de Homicídio Feminino CONSUMADO no ano de 2023 por Estado)  |                                                  
|  45  |  total_tentativas_homicidio  |  (Soma de todas as colunas de todos os anos de Homicídio Feminino TENTADO por Estado)  |                                     
|  46  |  total_homicidio_consumado  |  (Soma de todas as colunas de todos os anos de Homicídio Feminino CONSUMADO por Estado)  |                  
|  47  |  homicidios_2020  |  (Total de Homicídio Feminino ocorridos no ano de 2020)  |                                                
|  48  |  homicidios_2021  |  (Total de Homicídio Feminino ocorridos no ano de 2021)  |                                                  
|  49  |  homicidios_2022  |  (Total de Homicídio Feminino ocorridos no ano de 2022)  |                                                  
|  50  |  homicidios_2023  |  (Total de Homicídio Feminino ocorridos no ano de 2023)  |                                                  
|  51  |  total_feminicidios_2020  |  (Soma de Feminicídio TENTADO e CONSUMADO do ano de 2020)  |                                        
|  52  |  total_feminicidios_2021  |  (Soma de Feminicídio TENTADO e CONSUMADO do ano de 2021)  |                                        
|  53  |  total_feminicidios_2022  |  (Soma de Feminicídio TENTADO e CONSUMADO do ano de 2022)  |                                        
|  54  |  total_feminicidios_2023  |  (Soma de Feminicídio TENTADO e CONSUMADO do ano de 2023)  |                                          
|  55  |  total_feminicidios_2024  |  (Soma de Feminicídio TENTADO e CONSUMADO do ano de 2024)  |

  ### 📚 Ferramentas Utilizadas:
  
- [Google Colab](https://colab.research.google.com/drive/1kBkcopqrCuFdA_tWDo7EajIDLIsOxBSM?usp=sharing) para realizar a limpeza e a análise estatística dos dados.


- [Public Tableau](https://public.tableau.com/app/profile/carolyne.santos.de.oliveira/viz/on33-python-s17-s18-projeto-finalEstatsticaCriminaldoFeminicdionasUnidadesdaFederao/Apresentao2) dashboard e painel de visualização de dados.


- [PowerPoint](https://docs.google.com/presentation/d/1RHGsovdnWhP2myDpJVKSPxXjwzhzCGcH/edit?usp=drive_link&ouid=103014318842924902559&rtpof=true&sd=true) com a apresentação do projeto.


- [Video de Apresentação do Projeto](https://drive.google.com/file/d/1lZxBdchThomdWXp4tqIjX7Kd5q6aqgaS/view?usp=drive_link)


## 📈 Dashboard

Link para consulta do dashboard no Tableau Public:

[![dashboard](/Apresentacao.png)](https://public.tableau.com/app/profile/carolyne.santos.de.oliveira/viz/on33-python-s17-s18-projeto-finalEstatsticaCriminaldoFeminicdionasUnidadesdaFederao/Apresentao2)

## 📋 Passo a Passo

## 🟦 Análises:

Nesta base de dados, analisamos os registros de feminicídio, tanto tentado quanto consumado, no período de 2020 ao primeiro semestre de 2024. O gráfico abaixo apresenta a distribuição total de casos por região, permitindo uma visão clara da concentração dos incidentes ao longo dos anos.

![Total_Fem_Regi](/Graficos/Colab/Total_Fem_Regi.png)

O segundo gráfico apresenta um gráfico de pizza que ilustra a distribuição dos registros de feminicídio por região, proporcionando uma visão percentual clara de como os casos estão distribuídos geograficamente.

As regiões com maior numero de casos de feminicidio são:

- Sudeste, com um total de 4747 casos (27,4%).
- Nordeste, com um total de 4529 casos (26,1%).
- Sul com um total de 3349 casos (19,3%).
- Centro-Oeste com um total de 2440 casos (14,1%).
- Norte com um total de 2259 casos (13%).

![Distribui_Fem_Reg](/Graficos/Colab/Distribui_Fem_Reg.png)

Na terceira análise, comparamos a porcentagem de feminicídios dentro do total de homicídios femininos em cada estado.

Ao analisarmos os gráficos apresentados, é evidente o número alarmante de homicídios do gênero feminino. Contudo, uma parte desses casos se insere nas estatísticas de feminicídio. A análise revela que alguns estados brasileiros apresentam uma alta correlação entre homicídios femininos e feminicídios. Um exemplo notável é o Mato Grosso do Sul, que registra um total de 221 homicídios femininos, dos quais 155 são classificados como feminicídios, correspondendo a impressionantes 70,14% dos homicídios femininos no estado. Isso indica que mais de 70% desses casos são considerados feminicídios, também conhecidos como crimes de gênero. Outro exemplo é o estado de Santa Catarina que apresenta um total de 564 homicídios femininos, dos quais 289 são classificados como feminicídios, ou seja, correspondem a 51,24% dos homicídios femininos no estado.

![Comp_Fem_Hom](/Graficos/Colab/Comp_Fem_Hom.png)

No gráfico de linhas abaixo temos a evolução do número de feminicídios entre os anos de 2020 a 2023 por Estado.

Este gráfico ilustra um aumento consistente nos casos de feminicídio ao longo dos anos na maioria dos estados brasileiros. Essa tendência alarmante não apenas reflete a gravidade da situação, mas também destaca a necessidade urgente de ações eficazes para combater a violência de gênero. Além disso, a análise revela que algumas regiões apresentam um crescimento mais acentuado, indicando que o problema é multifacetado e pode ser influenciado por fatores sociais, econômicos e culturais específicos de cada estado. Portanto, é fundamental promover políticas públicas e iniciativas de conscientização que abordem essas questões de forma abrangente e eficaz.

![Evolucao_estados](/Graficos/Colab/Evolucao_estados.png)

Nos gráficos de barras abaixo, analisamos se os estados com as maiores taxas de desemprego também apresentam uma taxa elevada de feminicídios ao longo do ano de 2022.

Ao comparar os dois gráficos, observamos que os estados com a maior taxa de desemprego não coincidem com aqueles que apresentam os maiores índices de feminicídio. Isso indica que não podemos afirmar que existe uma relação direta entre uma alta taxa de desemprego e um aumento nos casos de feminicídio.

![taxa_desemp_fem_1](/Graficos/Colab/taxa_desemp_fem_1.png)

![taxa_desemp_fem_2](/Graficos/Colab/taxa_desemp_fem_2.png)

Nossa próxima análise examina a quantidade de delegacias especializadas no atendimento à mulher e as taxas de feminicídios por estado no ano de 2020.

A análise revela que os estados com o maior número de feminicídios em 2020 apresentam uma quantidade inadequada de delegacias especializadas em atender casos de violência de gênero. Essa discrepância é preocupante, pois a sub-representação de delegacias pode dificultar o acesso das vítimas à justiça e à proteção adequada. Além disso, a falta de recursos e treinamento específico para os profissionais dessas delegacias pode contribuir para a subnotificação dos casos e a impunidade. Portanto, é fundamental que haja um aumento na implementação de delegacias especializadas, acompanhadas de um investimento em capacitação e recursos, para garantir que as vítimas recebam o apoio necessário e que os casos de feminicídio sejam tratados com a seriedade que merecem.

![deleg_femin](/Graficos/Colab/deleg_femin.png)

O gráfico abaixo ilustra a redução no número de feminicídios por estado, comparando os anos de 2020 e 2023.

Na análise acima, observamos que, ao comparar os anos de 2020 e 2023, apenas três estados conseguiram reduzir o número de feminicídios: Rio Grande do Sul, Maranhão e Piauí. Além disso, o estado da Paraíba manteve a mesma quantidade de casos. Por outro lado, todos os outros estados apresentaram um aumento expressivo no número de feminicídios registrados.

![queda_crimes](/Graficos/Colab/queda_crimes.png)


 ### - Conclusão:

🌟 Esta análise evidenciou o crescimento preocupante do feminicídio no Brasil entre 2020 e 2024, com destaque para estados como Rio de Janeiro e São Paulo. 
Apesar dos avanços em políticas de combate à violência de gênero, como a criação de mais delegacias especializadas, ainda há grandes desafios a serem enfrentados, especialmente em regiões de alta vulnerabilidade. 
É crucial que políticas públicas sejam implementadas de forma mais equitativa e que o combate à violência de gênero seja uma prioridade contínua.
Reforçamos a importância de mais investimentos em proteção e conscientização, especialmente em áreas urbanas e rurais com altos índices de violência de gênero. 
Uma abordagem multifacetada é essencial para reduzir esses números e promover uma sociedade mais segura para todas as mulheres.
    
 ### - Links Uteis/Fontes:


🌎 [Mapa das Delegacias da Mulher](https://azmina.com.br/projetos/delegacia-da-mulher/)


🌎 [Monitor de Feminicídios da UEL1 (LESFEM)](https://sites.uel.br/lesfem/monitor-brasil/)


🌎 [O Fórum Brasileiro de Segurança Pública (FBSP)](https://forumseguranca.org.br/painel-violencia-contra-a-mulher/)


🌎 [O Atlas da Violência](https://www.ipea.gov.br/atlasviolencia/quem/3/sobre)


🌎 [Google DataSet](https://datasetsearch.research.google.com/search?src=0&query=feminic%C3%ADdio&docid=L2cvMTFrcGQyN3d4MQ%3D%3D)


🌎 [Base dos Dados](https://basedosdados.org/)


🌎 [IBGE](https://cidades.ibge.gov.br/brasil/pesquisa/10073/91256)


## 👩🏻‍🏫 Professora Patrícia Bongiovanni Catandi.


📖 [Material](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/S17S18-Projeto-Livre.pdf)


 [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/patriciacatandi)
