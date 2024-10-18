# 📈📉📊 Estatística Criminal do Feminicídio nas Unidades da Federação

[![pptx](/Capa_pptx.png)](https://docs.google.com/presentation/d/1RHGsovdnWhP2myDpJVKSPxXjwzhzCGcH/edit?usp=drive_link&ouid=103014318842924902559&rtpof=true&sd=true)

## 📚 Descrição da Atividade

Projeto Final semana 17/18.

**Objetivo:** Esta análise tem como objetivo demonstrar a evolução do crime de feminicídio por estado nos anos de 2020 a 2024. 
O feminicídio é definido como o assassinato de uma mulher em razão de seu gênero, 
frequentemente associado à violência doméstica, discriminação ou desigualdade de gênero. 
Além de traçar o crescimento desse crime ao longo dos anos, 
a análise também busca compará-lo com o número de homicídios femininos ocorridos nos estados e verificar a 
porcentagem de feminicídios em relação ao total de homicídios femininos. Com isso, pretende-se evidenciar a 
gravidade e o impacto específico da violência de gênero no contexto dos crimes contra a vida.

  ### 📚 Descrição da Base:

A escolha do tema e das bases de dados foi motivada pelo interesse em compreender quais fatores podem impactar diretamente o aumento ou a redução dos casos de feminicídio no Brasil.

Bases tratadas na aula da semana 17 [Feminicidio](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/database-Feminicidio.csv) 
e [Homicidios](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/homicidios_femininos.csv) disponiveis neste repositório.

Após tratamento minha base de dados ficou assim:
A base final de dados [FeminicidioPorEstado](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/feminicidio.csv) é composta por 56 colunas:

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
|  8  |  feminicidio_tentado_2024(LESFEM)  |  (Quantidade de Feminicidio TENTADO no ano de 2024 por Estado)  |
|  9  |  feminicidio_consumado_2024(LESFEM)  |  (Quantidade de Feminicidio CONSUMADO no ano de 2024 por Estado)  |
|  10  |  ano_2024  |  (Coluna do Ano de 2024)  |
|  11  |  feminicidio_tentado_2023(FBSP)  |  (Quantidade de Feminicidio TENTADO no ano de 2023 por Estado)  | 
|  12  |  feminicidio_consumado_2023(FBSP)  |  (Quantidade de Feminicidio CONSUMADO no ano de 2023 por Estado)  |
|  13  |  ano_2023  |  (Coluna do Ano de 2023)  | 
|  14  |  feminicidio_tentado_2022(FBSP)  |  (Quantidade de Feminicidio TENTADO no ano de 2022 por Estado)  |
|  15  |  feminicidio_consumado_2022(FBSP)  |  (Quantidade de Feminicidio CONSUMADO no ano de 2022 por Estado)  |
|  16  |  ano_2022  |  (Coluna do Ano de 2022)  |
|  17  |  feminicidio_tentado_2021(FBSP)  |  (Quantidade de Feminicidio TENTADO no ano de 2021 por Estado)  |
|  18  |  feminicidio_consumado_2021(FBSP)  |  (Quantidade de Feminicidio CONSUMADO no ano de 2021 por Estado)  |
|  19  |  ano_2021  |  (Coluna do Ano de 2021)  |
|  20  |  Feminicidio Tentado  |  (Quantidade de Feminicidio TENTADO no ano de 2020 por Estado)  | 
|  21  |  Feminicidio Consumado  |  (Quantidade de Feminicidio CONSUMADO no ano de 2020 por Estado)  |
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
|  37  |  tentativa_2020  |  (Quantidade de Homicidio Feminino TENTADO no ano de 2020 por Estado)  |                                              
|  38  |  consumado_2020  |  (Quantidade de Homicidio Feminino CONSUMADO no ano de 2020 por Estado)  |   
|  39  |  tentativa_2021  |  (Quantidade de Homicidio Feminino TENTADO no ano de 2021 por Estado)  |                                                   
|  40  |  consumado_2021  |  (Quantidade de Homicidio Feminino CONSUMADO no ano de 2021 por Estado)  |                                                  
|  41  |  tentativa_2022  |  (Quantidade de Homicidio Feminino TENTADO no ano de 2022 por Estado)  |                                                
|  42  |  consumado_2022  |  (Quantidade de Homicidio Feminino CONSUMADO no ano de 2022 por Estado)  |                                                  
|  43  |  tentativa_2023  |  (Quantidade de Homicidio Feminino TENTADO no ano de 2023 por Estado)  |                                                 
|  44  |  consumado_2023  |  (Quantidade de Homicidio Feminino CONSUMADO no ano de 2023 por Estado)  |                                                  
|  45  |  total_tentativas_homicidio  |  (Soma de todas as colunas de todos os anos de Homicidio Feminino TENTADO por Estado)  |                                     
|  46  |  total_homicidio_consumado  |  (Soma de todas as colunas de todos os anos de Homicidio Feminino CONSUMADO por Estado)  |                  
|  47  |  homicidios_2020  |  (Total de Homicidios Femininos ocorridos no ano de 2020)  |                                                
|  48  |  homicidios_2021  |  (Total de Homicidios Femininos ocorridos no ano de 2021)  |                                                  
|  49  |  homicidios_2022  |  (Total de Homicidios Femininos ocorridos no ano de 2022)  |                                                  
|  50  |  homicidios_2023  |  (Total de Homicidios Femininos ocorridos no ano de 2023)  |                                                  
|  51  |  total_feminicidios_2020  |  (Soma de Feminicidios TENTADO e CONSUMADO do ano de 2020)  |                                        
|  52  |  total_feminicidios_2021  |  (Soma de Feminicidios TENTADO e CONSUMADO do ano de 2021)  |                                        
|  53  |  total_feminicidios_2022  |  (Soma de Feminicidios TENTADO e CONSUMADO do ano de 2022)  |                                        
|  54  |  total_feminicidios_2023  |  (Soma de Feminicidios TENTADO e CONSUMADO do ano de 2023)  |                                          
|  55  |  total_feminicidios_2024  |  (Soma de Feminicidios TENTADO e CONSUMADO do ano de 2024)  |

  ### 📚 Ferramentas Utilizadas:
  
- [Google Colab](https://colab.research.google.com/drive/1kBkcopqrCuFdA_tWDo7EajIDLIsOxBSM?usp=sharing) para realizar a limpeza e a análise estatística dos dados.
</br>
- [Public Tableau](https://public.tableau.com/app/profile/carolyne.santos.de.oliveira/viz/on33-python-s17-s18-projeto-finalEstatsticaCriminaldoFeminicdionasUnidadesdaFederao/Apresentao2) dashboard e painel de visualização de dados.
</br>
- [PowerPoint](https://docs.google.com/presentation/d/1RHGsovdnWhP2myDpJVKSPxXjwzhzCGcH/edit?usp=drive_link&ouid=103014318842924902559&rtpof=true&sd=true) com a apresentação do projeto.
</br>
- [Video de Apresentação do Projeto](https://drive.google.com/file/d/1lZxBdchThomdWXp4tqIjX7Kd5q6aqgaS/view?usp=drive_link)
</br>

## 📈 Dashboard

Link para consulta do dashboard no tableau Public:

[![dashboard](/Apresentacao.png)](https://public.tableau.com/app/profile/carolyne.santos.de.oliveira/viz/on33-python-s17-s18-projeto-finalEstatsticaCriminaldoFeminicdionasUnidadesdaFederao/Apresentao2)

## 📋 Passo a Passo

## 🟦 Análises:

Nesta base de dados,

![Grafico1]( )

No segundo gráfico, 

![Grafico2]( )

Na terceira análise,.

![Grafico3]( )

No gráfico de barras

![Grafico4]( )

No gráfico de barras

![Grafico5]( )

Ao analisarmos a base de dados de forma diferente

![Grafico6]( )

No gráfico 

![Grafico7]( )

No gráfico de dispersão, 

![Grafico8]( )

No histograma abaixo,

![Grafico9]( )

No gráfico de barras abaixo, 

![Grafico10]( )

 ### - Conclusão:

🌟 Esta análise evidenciou o crescimento preocupante do feminicídio no Brasil entre 2020 e 2024, com destaque para estados como Rio de Janeiro e São Paulo. 
Apesar dos avanços em políticas de combate à violência de gênero, como a criação de mais delegacias especializadas, ainda há grandes desafios a serem enfrentados, especialmente em regiões de alta vulnerabilidade. 
É crucial que políticas públicas sejam implementadas de forma mais equitativa e que o combate à violência de gênero seja uma prioridade contínua.
Reforçamos a importância de mais investimentos em proteção e conscientização, especialmente em áreas urbanas e rurais com altos índices de violência de gênero. 
Uma abordagem multifacetada é essencial para reduzir esses números e promover uma sociedade mais segura para todas as mulheres.
    
 ### - Links Uteis:
</br>
🌎 [Mapa das Delegacias da Mulher](https://azmina.com.br/projetos/delegacia-da-mulher/)
</br>
🌎 [Monitor de Feminicídios da UEL1 (LESFEM)](https://sites.uel.br/lesfem/monitor-brasil/)
</br>
🌎 [O Fórum Brasileiro de Segurança Pública (FBSP)](https://forumseguranca.org.br/painel-violencia-contra-a-mulher/)
</br>
🌎 [O Atlas da Violência](https://www.ipea.gov.br/atlasviolencia/quem/3/sobre)
</br>
🌎 [Google DataSet](https://datasetsearch.research.google.com/search?src=0&query=feminic%C3%ADdio&docid=L2cvMTFrcGQyN3d4MQ%3D%3D)
</br>
🌎 [Base dos Dados](https://basedosdados.org/)
</br>

## 👩🏻‍🏫 Professora Patrícia Bongiovanni Catandi.
</br>
📖 [Material](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/S17S18-Projeto-Livre.pdf)
</br>
 [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/patriciacatandi)