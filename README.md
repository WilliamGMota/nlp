# NLP - Natural Language Processing
Esse repositório é para eu anotar os conceitos e códigos que utilizei para estudar NLP.
Como é um material de apoio, pode ser que algum conceito ainda não estava claro quando editei.


## Feature
É a composição de n-gramas + medida
feature = n-gramas + medida => Peso de uma palavra no conjunto de dados.

### N-Gramas
É a palavra ou uma sequência de palavra que será utilizado pelo algoritmo processar.
Eles podem ser
* __Unigramas__ que é somente uma palavra.
* __Bigramas__ que é o conjunto de duas palavras no texto, normalmente em sequência.
* __Trigramas__ que é o conjunto de três palavras no texto, normalmente em sequência.
* __Part of speach tagger__ que é uma parte do texto baseado em definição e contexto. (POS Taggers Stanford é um algorítmo que processa esse conceito).
* __Stop words__ são palavras que não adicionam muito sentido a frase.
* __Stemmer__ normalizaçao de palavras, stemmer é o processo que unificam palavras que são diferente mas possuem o mesmo significado, por exemplo, verbos conjugados.

### Medidas
* __Contagem de termos__
* __Frequência de termos__
* __Combinaçao de frequência de termos com o peso__ conhecido como __TD-IDF

## Análise de Sentimentos
Conteúdo textual que vai gerar com base feature, variável e derivativo

## Fluxo de Trabalho

### Para treino
1. Coleta de Dados
2. Limpeza de Dados
3. Aplicar Stemmer ou lematization, caso necessário
4. Criar n-gramas
5. Criar features
6. Selecionar algoritmo
7. Aplicar algoritmo
8. Avaliar resultado

### Aplicação
1. Capturar a frase ou documento
2. Acessar base construida
3. Classificar informaçao ou sugerir conteúdo.

__Nota:__ Sempre começao com um processo simples e ir aperfeiçoando o processo.

## API de exemplo - Classificação de conteúdo
No parâmetro query, informe o título da notícia e o algorítmo tentara classificar em:
carros, economia, educacao, esporte, musica, politica

https://classificacao-noticias.herokuapp.com/?query=<mensagem>

Modelo ModeloClassificacaoNoticias.ipynb

API na pasta apinoticias

### Vídeos e referência para Estudo
https://www.youtube.com/watch?v=ULmezlBTtQs&t=2393s
  
https://github.com/lucasloami/automatic_brain
  
wildml.com
