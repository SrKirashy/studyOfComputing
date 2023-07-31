# Assembly

*Todo hardware, mais especificamente a **CPU**, vem de fábrica entendendo um certo conjunto de instruções ou funções. Eles tem registradores que é como se fossem um tipo de memória.*

*Você coloca valores nesses registradores e chama uma instrução que é mais ou menos, a mesma coisa que chamar uma função passando argumentos.*

## Ex registrador:
```
MOV EAX, 5 ; // Coloca 5 no registrador EAX
ADD EAX, 6 ; // Soma 6 ao registrador EAX
```

## Ex função:
```
function soma(a, b) { return a + b }
soma(5, 6)
```

*Então a **CPU** executa alguma coisa e grava o resultado em outros registradores e você pode ler essa resposta.*

*A linguagem que usamos para falar diretamente com a máquina é **Assembly**, e seu montador, o **assembler**, traduz o código escrito em texto com mnemônicos com **JMP**, **ADD** ou **MOV**, diretamente nas instruções binárias da máquina.*