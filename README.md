# Digital Innovation One

_Código criado para utilização junto a plataforma da Digital Innovation One._

<p align="center"><img src="./DIO.png" width="500"></p>

## _Bootcamp Cognizant Cloud Data Engineer_

_Repositório de código do Dio Live Coding com AWS EMR e Python, relacionado a apresentação do desafio “Criando seu Ecossistema de Big Data na Nuvem”,  sob orientação do instrutor Cassiano Peres._

_Aqui contém os passos para a configuração na AWS e execução de análise de dados._

---

1. ## _Instruções_

   - Acesse S3: 

     https://s3.console.aws.amazon.com/s3/

     - Criar estrutura de data lake: *dio-live-datalake*
     - Criar estrutura de massas:
       - *dados*
       - *saída*
       - *temp*

   - Acesse o EMR: 

     https://console.aws.amazon.com/elasticmapreduce/

     - O cluster será criado pelo MrJob e não pelo console
     - Infraestrutura como código

   - Criar chave SSH

     - Acesse o Console do EC2: https://console.aws.amazon.com/ec2/ -> Pares de Chaves -> Criar Par de Chaves
     - Baixar arquivo .pem

   - Obter Id e chave secreta AWS para configurar MrJob

     - Perfil
     - Minhas credenciais de segurança: https://console.aws.amazon.com/iam/home?region={region}#/security_credentials
     - Chaves de acesso - Criar nova chave de acesso
     - Fazer download - única chance de visualizar

   - Ambiente linux

     - Criar ambiente virtual python: *virtualenv --python = python3.6 venv_diolive*
     - Acessar com o vs código

   - Instalar vscode no Ubuntu

     - código.

   - Criar algoritmo de análise de palavras

     - dio-live-wordcount-test.py
     - mapa-reduzir-contar: contar
     - Instalar boto3: *pip install boto3*
     - Instalar mrjob: *pip install mrjob*

   - Acessar S3

     - Upload de arquivo para o bucket

   - Ambiente virtual python: fonte venv_teste / bin / activate

     - *nano ~ / .mrjob.conf*
     - *python3 dio-live-wordcount-test.py -r emr s3: // {your_s3_bucket_name} /data/SherlockHolmes.txt --output-dir = s3: // {your_s3_bucket_name} / output / logs1 --cloud-tmp-dir = s3: // {your_s3_bucket_name} / temp /*

---

