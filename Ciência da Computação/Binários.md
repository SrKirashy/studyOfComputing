# Binários

***Binários** são sistemas de numeração que utilizam apenas dois símbolos para representar valores, geralmente os símbolos 0 e 1. Eles são a base fundamental da computação moderna e estão intimamente ligados ao funcionamento dos computadores e outros dispositivos eletrônicos.*

*O sistema **binário** é essencial porque os computadores digitais são baseados em circuitos eletrônicos que operam com dois estados distintos, como "ligado" e "desligado", ou "presença" e "ausência" de eletricidade. Os dígitos **binários** 0 e 1 são utilizados para representar esses dois estados.*

*Os computadores usam o sistema **binário** para processar e armazenar informações. Qualquer dado que você encontra em um computador, como textos, imagens, sons ou vídeos, é representado internamente em forma **binária.***

## Binários Na Prática


*Nós humanos, usamos dígitos que vão do 0 ao 9:*
```
    0 1 2 3 4 5 6 7 8 9
```
*Com esses 10 digitos, conseguimos fazer combinações como:*
```
    11, 25, 23, 54, 78, 254, 3564, 542, 74, etc.
```

----
*Porém os computadores são mais simples em certo sentido, eles utilizam um sistema de numeração **binária**, que vai do 0 até 1:*

```
    0 1
```
*E com esses dois números ele cria combinações como:*

```
    11010
```
*O **binário** "11010" é o número "26".*



## Converção 

*Para fazer a conversão, começamos dividindo o número decimal por 2 e anotando o resto da divisão. Em seguida, continuamos dividindo o quociente da divisão anterior até chegarmos a um quociente igual a 0. A representação **binária** é construída lendo-se os restos de baixo para cima.*

*Passo a passo:*
```
    26 dividido por 2 resulta em 13 com resto 0.
    13 dividido por 2 resulta em 6  com resto 1.
    6  dividido por 2 resulta em 3  com resto 0.
    3  dividido por 2 resulta em 1  com resto 1.
    1  dividido por 2 resulta em 0  com resto 1.
```

*Agora, lemos os restos de baixo para cima: 11010. Portanto, o número decimal "26" em **binário** é representado como "11010".*



Assim, a conversão do número decimal "26" para **binário** é correta.

## Verificação

*Temos o número decimal "26" que foi convertido para **binário** e obtivemos "11010". Agora, queremos verificar se a conversão está correta.*

*A representação binária "11010" é formada por cinco **dígitos binários**, cada um representando uma potência de 2. Os **dígitos** estão dispostos da direita para a esquerda, sendo o último **dígito** (à direita) o 2^0, o penúltimo o 2^1, e assim por diante.*

*A fórmula para converter um número binário em decimal é a seguinte:*
```
    Número Decimal = (d1 * 2^0) + (d2 * 2^1) + (d3 * 2^2) + (d4 * 2^3) + ... + (dn * 2^(n-1))
```
*Onde:
d1, d2, d3, ... dn são os **dígitos binários**, sendo d1 o dígito menos significativo (último à direita) e dn o dígito mais significativo (primeiro à esquerda).*

*Agora, usando o exemplo "11010":*
```
    Número Decimal = (0 * 2^0) + (1 * 2^1) + (0 * 2^2) + (1 * 2^3) + (1 * 2^4)

    Número Decimal = 0 + 2 + 0 + 8 + 16

    Número Decimal = 26
```

*Concluímos que a conversão está correta porque a soma dos valores dos dígitos binários (0, 1, 0, 1 e 1) multiplicados pelas potências de 2 resulta em 26, que é exatamente o número decimal original que desejávamos converter.*

*Essa é a lógica por trás da verificação da conversão de binário para decimal, e ela pode ser aplicada a qualquer outro número binário convertido para decimal para garantir a precisão da conversão.*

## E como armazenamos texto em binário?

*Quando você se refere a "um texto em **binário**", geralmente isso significa que o texto foi codificado usando a representação **binária** dos caracteres. Cada caractere do texto é representado por uma sequência única de bits (0s e 1s) de acordo com um padrão de codificação específico, como o **ASCII (American Standard Code for Information Interchange)** ou o **UTF-8*** **(Unicode Transformation Format - 8 bits)**.*

*No **sistema binário**, cada caractere é atribuído a um número único, que é chamado de **"código binário"** ou **"valor binário"**. Por exemplo, no padrão **ASCII**, o caractere "A" é representado pelo valor **binário** 01000001, o caractere "B" pelo valor **binário** 01000010 e assim por diante.*

*Portanto, para representar um texto em **binário**, você precisa converter cada caractere do texto em sua respectiva representação **binária** de acordo com o padrão de codificação usado. A sequência de **bits** obtida após a conversão de todos os caracteres do texto forma o texto em binário.*

*Por exemplo, vamos converter o texto "HELLO" em binário usando o padrão ASCII:*
```
    H -> Valor ASCII: 72 -> Representação binária: 01001000
    E -> Valor ASCII: 69 -> Representação binária: 01000101
    L -> Valor ASCII: 76 -> Representação binária: 01001100
    L -> Valor ASCII: 76 -> Representação binária: 01001100
    O -> Valor ASCII: 79 -> Representação binária: 01001111
```
*O texto "HELLO" em binário usando o padrão ASCII é:*
```
    01001000 01000101 01001100 01001100 01001111
```

*Assim, cada caractere é representado por sua sequência binária única, permitindo que o computador armazene, transmita e processe o texto usando a linguagem dos números **binários**. Essa é uma das bases fundamentais para o funcionamento da computação e da transmissão de dados digitais.*