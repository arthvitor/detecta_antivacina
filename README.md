# Detector de tweets Antivacina
Esse repositório são conjuntos de dados, códigos, análises e gráficos de um detector automatico, usando aprendizado de máquina supervisionado, de possíveis tweets antivacina ou pró-vacina. Esse script, dividido em três notebooks, tem as tarefas de extração direta na API do Twitter, usando conta de desenvolvedor, aprendizado de máquina usando os algoritmos ```NaiveBayesClassifier```, ```MaxentClassifier``` e ```SklearnClassifier```. 

## Como começar?
1. Abrindo o notebook ```projeto_antivacina_coleta.ipynb```, colocando sua chave da API do Twitter para realizar a extração. É preferêncial que o plano da conta de desenvolvedor do Twitter seja Elevated ou superior;
2. Abrindo o notebook ```projeto_antivacina_treinamento.ipynb```, recebendo os arquivos das extrações e de treino para conseguir treinar os algoritmos de machine learning. Caso queria ter o mesmo resultado dessa análise, abra os arquivos que se encontram na pasta ```data```;
3. Abrindo o notebook ```projeto_antivacina_aed.ipynb```, recebendo os arquivos já analisados. Para replicabilidade, utilize o arquivo analisado da pasta ```data```.

## Sobre a coleta
A coleta foi realizada no endpoint ```/2/tweets/search/recent```, da APIv2 do Twitter. Devido a um bug da API, somente as ids dos autores foram coletadas. As linhas não tem os nomes dos usuários. 

## Sobre os arquivos

### ```corpus_anti.data``` (antivácina) | ```corpus_pro.data``` (pro-vácina) | ```corpus_neu.data``` (neutro)  
Arquivos de entrada para realização do treino dos algoritmos de aprendizado de máquina

### ```corpus_treino.csv``` | ```corpus_treino2.csv```
Arquivos de amostras usado para realizar a classificação manual e extrair um corpus de treino para o aprendizado de máquina

### ```dataset1.csv``` | ```dataset2.csv```
Arquivos da captura de tweets do endpoint ```/2/tweets/search/recent```

### ```tweets_classificados.csv```
Arquivo com tweets já classificados

### ```projeto_antivacina_x```
Arquivos com os códigos em python para execução da análise

### arquivos na pasta ```gráficos```
Arquivos em HTML com os gráficos já plotados pelo vegas studio

## Contato
Caso tenha dúvidas sobre esse script e análise, mande um e-mail para **vitorarthur.profissional@gmail.com**

## Finalidade do projeto
Trabalho realizado como projeto final da disciplina Pensamento Computacional, do Master em Jornalismo de Dados, Automação e Data Storytelling do Insper.

