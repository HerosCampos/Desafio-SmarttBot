# Desafio SmarttBot

Olá, para a realização deste desafio foi utilizado o arquivo CSV disponível no link enviado, caso seja necessário atualizar o link ou trocar de Dataset gentileza me informar que eu realizo a atualização :).

O arquivo se chama: 
* bitstampUSD_1-min_data_2012-01-01_to_2020-09-14.csv (disponível no link 
https://www.kaggle.com/mczielinski/bitcoin-historical-data/data#coinbaseUSD_1-min_data_2014-12-01_to_2019-01-09.csv)

Para organizar as etapas eu coloquei os meus objetivos em um quadro, utilizei o excelente livro chamado Manual de Análise Técnica do autor Marcos Abe para fazer algumas pesquisas e recorri diversas vezes ao Google.
A organização das ideias ficou assim:
![20201205_121434](https://user-images.githubusercontent.com/73557900/101296192-d6cf5700-3800-11eb-9c27-7d835a964342.jpg)

Procurei anotar e deixar registrado os principais pontos no Jupyter Notebook então irei utilizar este Read Me para complementar o que considero importante.

![datas](https://user-images.githubusercontent.com/73557900/101296460-907af780-3802-11eb-8872-ad7366459646.PNG)
* No arquivo em .pdf que me foi enviado, no campo 'Orientações' estava solicitando que fosse possível escolher as datas de início e de fim, neste caso é possível escolher a visualização pelas datas de forma bruta Ex: AAAA-MM-DD ou utilizando as datas junto com as horas, minutos e segundos Ex: AAAA-MM-DD HH:MM:SS.

---

No gif a seguir mostro o que considero ser o maior ponto fraco do projeto, consegui criar um gráfico interativo de candles mas não consegui adicionar as Médias Móveis Exponenciais e nem as Bandas de Bollinger. Tive que gerar os gráficos das MME e da BB com gráfico de linhas, ficou legal mas não tão legal :/
PS: Pode juntar este gráfico com o IFR pois o gráfico de Índice de Força Relativa é visualizado de forma 'separada', como no exemplo que mostro no Jupyter Notebook.
![candles](https://user-images.githubusercontent.com/73557900/101296863-9540ab00-3804-11eb-9b90-0db682142cda.gif)

---
* Também é possível configurar as Médias Móveis Exponenciais, você escolhe os períodos desejados e elas são atualizadas (inclusive na legenda) no gráfico. 
* Para esta estratégia eu utilizei um sistema simples de cruzamento de MME, mas, caso essa não seja uma estratégia de preferência do usuário ele pode optar por não gerar os demais comandos, ficando apenas com as MME.
* Caso o usuário opte por utilizar o sistema de cruzamento de Médias Móveis Exponenciais ele receberar algumas 'dicas' de compra ou venda assim que as médias se cruzarem.

![MME](https://user-images.githubusercontent.com/73557900/101296933-0e400280-3805-11eb-993c-71a4bb8662e3.PNG)

---

É possível salvar o CSV de duas formas:
1. A tabela completa, inclusive com os valores de Fechamento dos preços.
2. A tabela simplificada, apenas com o timestamp e os indicadores (como foi solicitado no pdf).

---
Me diverti muito realizando este desafio, caso seja necessário eu posso trocar o DataSet e atualizar o código, posso criar o programa no VS Code...
Muito obrigado
![129050381_3470516109733082_64953203074297752_n](https://user-images.githubusercontent.com/73557900/101297361-5d873280-3807-11eb-955f-2ecbae1ecef8.jpg)
