# Perceptron

## 1. Conceito
Explique, com suas palavras, o que é um Perceptron e qual a sua importância histórica para o desenvolvimento da Inteligência Artificial.

Perceptron é o nome dado ao modelo que seria o primeiro neurônio artificial, dividido entre quatro partes: entradas, conexões, corpo da célula e saída. É um modelo que tem como resultado binário, através da distribuição dos valores das entradas e seus respectivos pesos, seguido com um valor constante pra calibrar o resultado, chamado Bias. Esse modelo foi de grande importância histórica, pois abriu portas pra criação de redes neurais artificiais, fazendo com que as máquinas fossem capazes de aprender padrões a partir de exemplos.

## 2. Funcionamento
O Perceptron é considerado um classificador linear. O que isso significa? Quais são as limitações desse tipo de modelo?

Ser considerado como um classificador linear quer dizer que o modelo consegue decidir e separar algo entre uma classe A ou B (Apto/Não Apto, Sim/Não, Feio/Bonito, Alto/Baixo). Entretanto, sua limitação está no fato de que se existirem variáveis que, ao ser combinadas, não chegam num denominador comum entre a classe A ou B, a resposta não é precisa.

## 3. Código
Ao analisar o código que você executou, quais foram as etapas principais do processo de treinamento do Perceptron?

Na primeira etapa do código, foi realizada criação do método `main()`, que além de exibir as mensagens “Hello World!” e “This is the main file”, expõe o resultado final do perceptron com a invocação do outro método `perceptron_input()`.

Em seguida, foi criado o método `perceptron_input()`, que nos seus parâmetros o usuário coloca os valores dos inputs, dos pesos e do Bias - assim respectivamente. Nesse método, é calculada a soma ponderada dos valores estabelecidos pelo usuário - os inputs e pesos formam “duplas” de acordo com suas posições na lista, e calculam o produto entre eles, logo em seguida é somado esses valores; o valor encontrado é somado com o valor do Bias, gerando assim seu valor final.

Por fim, foi realizada o método `perceptron_output`, que faz a calibragem final do perceptron, distinguindo em valores binários o resultado final do perceptron. Nesse código, se o valor do método `perceptron_input()` for igual ou maior que zero, seu valor binário será 1, e todos os valores diferentes disso o valor binário será 0.

## 4. Aplicação prática
Dê um exemplo real em que o uso de um modelo simples como o Perceptron poderia ser útil. Justifique sua escolha.

Um exemplo real onde um modelo simples como o Perceptron poderia ser útil é em um sistema de triagem para vaga de estágio para o setor de RH de uma empresa. O objetivo seria criar um filtro automático inicial para filtrar um alto volume de currículos, que seria inviável analisar manualmente. Nesse sistema, variáveis como nível de proficiência em idiomas (Básico, Intermediário, Avançado, Fluente) são convertidas em valores de 1 a 4. Outro exemplo seria criar um ranking de 1 a 5 para universidades com base em classificações de mercado, permitindo que a empresa priorize candidatos de instituições que historicamente formam profissionais com o perfil desejado.