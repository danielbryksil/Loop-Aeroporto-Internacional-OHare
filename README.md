# Loop-Aeroporto-Internacional-OHare

## Descrição do Projeto
Como analista da empresa fictícia Zuber, uma nova empresa de compartilhamento de caronas que está sendo lançada em Chicago. Minha tarefa é encontrar padrões nas informações disponíveis. Entender as preferências dos passageiros e o impacto de fatores externos nas corridas. Trabalhando com um banco de dados, analisei dados de concorrentes e testei uma hipótese sobre o impacto do clima na frequência das viagens.

## Descrição dos dados
Um banco de dados com informações sobre corridas de táxi em Chicago:

tabela neighborhoods: dados sobre os bairros da cidade
-	name: nome do bairro
-	neighborhood_id: código do bairro

tabela cabs: dados sobre os táxis
-	cab_id: código do veículo
-	vehicle_id: a identificação técnica do veículo
-	company_name: a empresa proprietária do veículo

tabela trips: dados sobre corridas
-	trip_id: código da corrida
-	cab_id: código do veículo que opera a corrida
-	start_ts: data e hora do início da corrida (tempo arredondado para a hora)
-	end_ts: data e hora do final da corrida (tempo arredondado para a hora)
-	duration_seconds: duração da corrida em segundos
-	distance_miles: distância percorrida em milhas
-	pickup_location_id: código do bairro de retirada
-	dropoff_location_id: código do bairro de entrega

tabela weather_records: dados sobre o clima
-	record_id: código de registro meteorológico
-	ts: grava data e hora (tempo arredondado para a hora)
-	temperature: temperatura quando o registro foi feito
-	description: breve descrição das condições meteorológicas, ex. "chuva leve" ou "nuvens esparsas"

## Instruções do projeto

1. Análise Exploratória de Dados
- Encontrar o número de corridas de táxi para cada empresa de táxi de 15 a 16 de novembro de 2017. Nomear o campo resultante como trips_amount e imprima-o junto com o campo company_name. Ordenar os resultados pelo campo trips_amount em ordem decrescente.
- Encontrar o número de corridas para cada empresa de táxi cujo nome contém as palavras "Amarelo" ou "Azul" de 1º a 7 de novembro de 2017. Nomear a variável resultante como trips_amount. Agrupar os resultados pelo campo company_name.
- Em novembro de 2017, as empresas de táxi mais populares eram Flash Cab e Taxi Affiliation Services. Encontrar o número de corridas para essas duas empresas e nomeie a variável resultante como trips_amount. Juntar as corridas para todas as outras empresas no grupo "Outros". Agrupar os dados por nomes de empresas de táxi. Nomear o campo com os nomes das empresas de táxi como company. Classifique o resultado em ordem decrescente por trips_amount.

2. Testar a hipótese de que a duração das corridas do Loop até ao Aeroporto Internacional O'Hare muda em sábados chuvosos.

