# Redes-Neurais-com-Keras

# Integrantes
- André Geraldi Marcolongo, RM555285 - 2TDSPV
- Eduardo Guilherme Dias, RM557886 - 2TDSPV
- Luiz Felipe Campos da Silva - RM555591 - 2TDSPV
- Pedro Abrantes Andrade - RM558186 - 2TDSPV

## Baixe o arquivo:
`cp5-parte1-IA.ipynb`

## Acesse o arquivo via Google Colab ou Jupyter Notebook
``` bash
jupyter notebook cp5-parte1-IA.ipynb
```
**Instale as bibliotecas necessárias para rodar as células do arquivo**

## Comparação de desempenho entre modelos
### Exercício 1 - CLASSIFICAÇÃO MULTICLASSE
#### Acurácia e perdas treinando Rede Neural com Keras:
<img width="635" height="150" alt="image" src="https://github.com/user-attachments/assets/471ebf2b-6685-4079-8e5d-0ad8d7c68921" />

#### Acurácia treinando com RandomForest:
<img width="632" height="202" alt="image" src="https://github.com/user-attachments/assets/e24e4668-f159-4f31-a32d-b2f9753c231e" />

#### Análise:
Observamos o melhor desempenho utilizando o modelo RandomForest, mas desconfiamos de um possível overfitting, por conta da acurácia em 100%. Já o modelo Keras, apresentou uma acurácia equilibrada

### Exercício 2 - REGRESSÃO
#### RMSE e perdas treinando Rede Neural com Keras:
<img width="1089" height="194" alt="image" src="https://github.com/user-attachments/assets/01126370-169d-40a2-a71c-d86b0494799d" />

#### RMSE treinando com LinearRegression:
<img width="1499" height="418" alt="image" src="https://github.com/user-attachments/assets/299bb7ad-676c-4c28-acf5-c985dcbfdef0" />

#### Análise:
**Porquê a Rede Neural performou melhor que o modelo de Regressão Linear?**

Modelos de Regressão Linear assumem uma relação linear entre as características de entrada e a variável alvo. Isso significa que eles tentam encontrar a melhor linha reta (ou hiperplano em dimensões superiores) para ajustar os dados.

Redes neurais, por outro lado, são capazes de aprender e modelar relações muito mais complexas e não lineares. Elas fazem isso através de suas múltiplas camadas e funções de ativação, que lhes permitem capturar padrões intrincados que um modelo linear simples não consegue.

No caso do conjunto de dados California Housing, é provável que a relação entre fatores como renda média, idade da casa, número de quartos, população, etc., e o valor médio da casa não seja estritamente linear. Provavelmente há interações e efeitos não lineares em jogo. Como sua rede neural tem a capacidade de aprender esses padrões não lineares, ela pode fazer previsões mais precisas, resultando em um RMSE menor em comparação com o modelo de Regressão Linear.

Pense nisso como tentar ajustar uma curva complexa com uma linha reta versus ajustá-la com uma linha flexível e curvilínea. A linha curvilínea (a rede neural) pode seguir a forma dos dados mais de perto.
