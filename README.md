# kafka-demo
demonstração básica de um serviço de Producer e Consumer com Apache Kafka, C# e .NET
# Executando o projeto

## Pré-requisitos

<br>-.Net 5.0</br>
<br>-Docker</br>
<br>-Offset Explorer</br>

## Configuração do Offset Explorer
bootstrap servers = localhost:9092
Zookeper Host=localhost Port=2181

Ou troque para a porta que estiver utilizando nas configurações do projeto e docker

## Execução
<br>-na pasta "docker-kafka" execute o comando "docker compose up -d" para executar a imagem da confluente (necessário ter o Docker instalado) e caso prefira pode seguir o **[guia quick start da Confluent](https://docs.confluent.io/platform/current/get-started/platform-quickstart.html)**</br>

<br>-No arquivo "Program.cs" escolha qual serviço será executado (Consumer ou Producer) comentando as linhas 34 ou 35 e deixando sem comentários, apenas a linha referente ao serviço que será executado (começar pelo Producer).</br>
<br>-Executar a aplicação com o serviço de Producer.</br>
<br>-Acompanhe quais mensagens foram produzidas pela GUI do Offset Explorer. Clique na conexão criada anteriormente e no nome do tópico que foi configurado no arquivo 'appsettings.json' do projeto. Depois no botão com o ícone de execução para poder listar todas as mensagens produzidas.</br>
<br>-Troque os comentários do arquivo "Program.cs" para utilizar o serviço de Consumer e execute o programa novamente para ver as mensagens sendo consumidas.</br>

## Demonstração em vídeo
-Em caso de dúvidas assista a **[demonstração em vídeo ](https://youtu.be/zE-ePHHeBWQ)** da execução do projeto.

