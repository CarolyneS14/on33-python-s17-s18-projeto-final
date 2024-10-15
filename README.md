# 📈📉📊 Estatística Criminal do Feminicídio nas Unidades da Federação

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

Bases tratadas na aula da semana 17 [Feminicidio](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/database-Feminicidio.csv) 
e [Homicidios](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/homicidios_femininos.csv) disponiveis neste repositório.

Após tratamento minha base de dados ficou assim:
A base final de dados [FeminicidioPorEstado](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/feminicidio.csv) é composta por 56 colunas:

 0   estado                                                         27 non-null     object 
 1   siglas                                                         27 non-null     object 
 2   regiao                                                         27 non-null     object 
 3   total_municipos_por_estado(IBGE)                               27 non-null     int64  
 4   renda_per_capita(IBGE)                                         27 non-null     int64  
 5   idh(IBGE)                                                      27 non-null     float64
 6   taxa_desemprego_feminino                                       27 non-null     float64
 7   delegacias_especializadas_de_atendimento_a_mulher              27 non-null     int64  
 8   feminicidio_tentado_2024(LESFEM)                               27 non-null     int64  
 9   feminicidio_consumado_2024(LESFEM)                             27 non-null     int64  
 10  ano_2024                                                       27 non-null     int64  
 11  feminicidio_tentado_2023(FBSP)                                 27 non-null     int64  
 12  feminicidio_consumado_2023(FBSP)                               27 non-null     int64  
 13  ano_2023                                                       27 non-null     int64  
 14  feminicidio_tentado_2022(FBSP)                                 26 non-null     float64
 15  feminicidio_consumado_2022(FBSP)                               27 non-null     int64  
 16  ano_2022                                                       27 non-null     int64  
 17  feminicidio_tentado_2021(FBSP)                                 25 non-null     float64
 18  feminicidio_consumado_2021(FBSP)                               27 non-null     int64  
 19  ano_2021                                                       27 non-null     int64  
 20  Feminicidio Tentado                                            23 non-null     float64
 21  Feminicidio Consumado                                          27 non-null     int64  
 22  ano_2020                                                       27 non-null     int64  
 23  indicador_conferencia_politicas_para_mulheres                  27 non-null     object 
 24  %_total_numero_municipios_conferencia_politicas_para_mulheres  27 non-null     float64
 25  numero_municipios_conferencia_politicas_para_mulheres          27 non-null     int64  
 26  indicador_protecao_vitimas_violencia                           27 non-null     object 
 27  %_total_numero_municipios_protecao_vitimas_violencia           27 non-null     float64
 28  numero_municipios_protecao_vitimas_violencia                   27 non-null     int64  
 29  indicador_lei_especifica_violencia                             27 non-null     object 
 30  %_total_numero_municipios_lei_especifica_violencia             27 non-null     float64
 31  numero_municipios_lei_especifica_violencia                     27 non-null     int64  
 32  indicador_prog_específicas_para_mulheres                       27 non-null     object 
 33  %_total_numero_municipios_prog_específicas_para_mulheres       27 non-null     float64
 34  numero_municipios_prog_específicas_para_mulheres               27 non-null     int64  
 35  indicador_acoes_PM                                             27 non-null     object 
 36  acoes_junto_a_PM                                               27 non-null     object 
 37  tentativa_2020                                                 27 non-null     int64  
 38  consumado_2020                                                 27 non-null     int64  
 39  tentativa_2021                                                 27 non-null     int64  
 40  consumado_2021                                                 27 non-null     int64  
 41  tentativa_2022                                                 27 non-null     int64  
 42  consumado_2022                                                 27 non-null     int64  
 43  tentativa_2023                                                 27 non-null     int64  
 44  consumado_2023                                                 27 non-null     int64  
 45  total_tentativas_homicidio                                     27 non-null     int64  
 46  total_homicidio_consumado                                      27 non-null     int64  
 47  homicidios_2020                                                27 non-null     int64  
 48  homicidios_2021                                                27 non-null     int64  
 49  homicidios_2022                                                27 non-null     int64  
 50  homicidios_2023                                                27 non-null     int64  
 51  total_feminicidios_2020                                        23 non-null     float64
 52  total_feminicidios_2021                                        25 non-null     float64
 53  total_feminicidios_2022                                        26 non-null     float64
 54  total_feminicidios_2023                                        27 non-null     int64  
 55  total_feminicidios_2024

  ### 📚 Ferramentas Utilizadas:
  
- [Google Colab](https://colab.research.google.com/drive/1kBkcopqrCuFdA_tWDo7EajIDLIsOxBSM?usp=sharing) para realizar a limpeza e a análise estatística dos dados.
- [Public Tableau](https://public.tableau.com/app/profile/carolyne.santos.de.oliveira/viz/on33-python-s17-s18-projeto-finalEstatsticaCriminaldoFeminicdionasUnidadesdaFederao/Apresentao) dashboard e painel de visualização de dados.
- [PowerPoint](https://docs.google.com/presentation/d/1-cumN-GNFIULjQmLKfj6SaBLprnBsW-P/edit?usp=drive_link&ouid=103014318842924902559&rtpof=true&sd=true)
- [Video Apresentacao](https://drive.google.com/file/d/1lZxBdchThomdWXp4tqIjX7Kd5q6aqgaS/view?usp=drive_link)

## 📈 Dashboard

Link para consulta do dashboard no tableau Public:

[Dashboard Feminicidio Por Estado](https://public.tableau.com/app/profile/carolyne.santos.de.oliveira/viz/on33-python-s17-s18-projeto-finalEstatsticaCriminaldoFeminicdionasUnidadesdaFederao/Apresentao)

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

🌟 
    
 ### - Links Uteis:

🌎 [Mapa das Delegacias da Mulher](https://azmina.com.br/projetos/delegacia-da-mulher/)
🌎 [Monitor de Feminicídios da UEL1 (LESFEM)](https://sites.uel.br/lesfem/monitor-brasil/)
🌎 [O Fórum Brasileiro de Segurança Pública (FBSP)](https://forumseguranca.org.br/painel-violencia-contra-a-mulher/)
🌎 [O Atlas da Violência](https://www.ipea.gov.br/atlasviolencia/quem/3/sobre)
🌎 [Google DataSet](https://datasetsearch.research.google.com/search?src=0&query=feminic%C3%ADdio&docid=L2cvMTFrcGQyN3d4MQ%3D%3D)
🌎 []()
🌎 []()

## 👩🏻‍🏫 Professora Patrícia Bongiovanni Catandi.
[GitHub](https://github.com/patriciacatandi "Patricia Catandi")

[Material](https://github.com/CarolyneS14/on33-python-s17-s18-projeto-final/blob/main/S17S18-Projeto-Livre.pdf)
