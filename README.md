# 1. Introdução

## 1.1. O que é Machine Learning

Machine Learning (*ML*) é um subcampo da ciência da computação que se preocupa em cronstruir algoritmos que, para serem úteis, dependem da coleção de exemplos de algum fenômeno.

ML também pode ser definido como o processo de resolver um problema prático por meio de **(1)** coleta de um conjunto de dados (*dataset*), e **(2)** construção algorítmica de um modelo estatístico com base nesse dataset.

## 1.2. Tipos de Aprendizado

Aprendizado pode ser supervisionado, semi-supervisionado, não-supervisionado e por reforço.

### 1.2.1. Aprendizado Supervisionado

No *aprendizado supervisionado*, o dataset é a coleção de exemplos rotulados (*labels*) ![CodeCogsEqn](https://github.com/user-attachments/assets/b4834277-c39b-4eac-9c24-cd1b29edf789).

Cada elemento ![CodeCogsEqn (1)](https://github.com/user-attachments/assets/52d461b9-15cf-4c20-8948-284310dd4a38) entre os *N* é chamado de **vetor de características** (*features*). Um vetor de features é um vetor no qual cada dimensão *j*=1,...,D contém um valor que descreve o exemplo de alguma forma. Esse valor é chamado de **característica** e é denotado como ![CodeCogsEqn (2)](https://github.com/user-attachments/assets/30d76e65-88ca-4e43-8e04-245da3a3a19e). Por exemplo, se cada exemplo x em nossa coleção representar uma pessoa, então a primeira característica, ![CodeCogsEqn (3)](https://github.com/user-attachments/assets/208fbbde-b1bb-4c25-ad31-5845c61692f6), poderia conter a altura em cm, a segunda característica, ![CodeCogsEqn (4)](https://github.com/user-attachments/assets/2bec122d-2e69-47e0-9ac5-3c24bd1fdc1b), poderia conter o peso em kg e assim por diante. Para todos os exemplos no conjunto de dados, a característica na posição *j* do vetor de características sempre contém o mesmo tipo de informação. Isso significa que, se ![CodeCogsEqn (5)](https://github.com/user-attachments/assets/960f9db1-6cd9-4e01-977f-9faaf3125e9c) contém o peso em kg em algum exemplo ![CodeCogsEqn (6)](https://github.com/user-attachments/assets/95bbef62-daa9-4a58-9010-3d53bd1a02ba), então ![CodeCogsEqn (7)](https://github.com/user-attachments/assets/ce811af6-47be-4cd3-bc2e-023a2dc6a4ab) também conterá o peso em kg em todo exemplo ![CodeCogsEqn (8)](https://github.com/user-attachments/assets/2dfd0711-8911-48f3-b6a9-96557e66396f), *k*=1,...,N.

O rótulo ![CodeCogsEqn (9)](https://github.com/user-attachments/assets/bede3f37-f5ba-4ae8-b3cb-496ef236e3cd) pode ser um elemento pertencente a um conjunto finito de classes {1,2,...,C}, um número real ou uma estrutura mais complexa, como um vetor, uma matriz, uma árvore ou um grafo. Você pode ver uma classe como uma categoria à qual um exemplo pertence. Por exemplo, se seus exemplos são mensagens de e-mail e seu problema é a detecção de spam, então você tem duas classes: {spam, não_spam}.

* O objetivo de um algoritmo de aprendizado supervisionado é usar o dataset para produzir um *modelo* que receba um vetor de features x como entrada e forneça informações que permitam deduzir o rótulo para esse vetor de features. Por exemplo, o modelo criado usando o dataset de pessoas poderia receber como entrada um vetor de features que descreve uma pessoa e fornecer a probabilidade de que essa pessoa tenha câncer.

