# PharmacIA 

Análise de apresentações(strings) de medicamentos baseada em PLN (Processamento de Linguagem Natural). 

PhamarcIA utiliza a biblioteca Spacy para a classificação das apresentações dos medicamentos, sendo  aquela uma biblioteca utilizada para processamento avançado de linguagem natural. 

Apresentação de um medicamento é um termo técnico para designar uma string que contém informações relativas ao medicamento. Neste projeto, as informações que serão trabalhadas seguem o formato: o nome do fabricante, o nome do medicamento, a concentração, a forma (comprimido, solução oral, etc.) e a quantidade. Outras informações não são de importância para a classificação. 
A seguir temos um exemplo de uma apresentação de um medicamento: 

**Cimed Indústria de Medicamentos Ltda Nimesulida 100 MG COM CT BL AL PLAS TRANS X 12** 

Então temos: 

- Nome do fabricante: Cimed Indústria de Medicamentos Ltda 
- Nome do medicamento: Nimesulida 
- Concentração: 100 MG 
- Forma: COMP (comprimido) 
- Quantidade: 12 (comprimidos) 

O Spacy trabalha com a classificação de termos baseada em tags. As marcações(tags) que foram feitas no arquivo "mapeamentos_medicamentos", que servem para treinar o modelo, podem ser melhor compreendidas a partir da leitura do artigo [Python for NLP: Parts of Speech Tagging and Named Entity Recognition](https://stackabuse.com/python-for-nlp-parts-of-speech-tagging-and-named-entity-recognition/) e da documentação do [Spacy](https://spacy.io/usage/linguistic-features).
