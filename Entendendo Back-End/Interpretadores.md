# O que é um Interpretador?
*Um programa, cuja sua função é ler código escrito, e traduzir em instruções pra máquina, sem necessariamente precisar compilar esse código em binário nativo. Ou seja, ele depende de ter o código-fonte do seu programa, e traduzir ou interpretar o código, toda vez que carrega.*

*Ele contém partes de um compilador, como o **parser**, para interpretar o código que você escreveu precisamos de um programa que leia esse código e interprete conforme a gramática da linguagem, e traduza isso em instruções de máquina ou uma representação similar. Para isso serve o **parser**.*

*Pode ser um pouco complicado entender, mas originalmente um interpretador é só um programa, como dito anteriormente. Você executa na linha de comando, e passa como argumento um caminho para um arquivo de texto que contém o código que você escreveu, na linguagem que esse interpretador entende. Ele vai carregar esse arquivo, vai usar o **parser**, para verificar se você escreveu corretamente, vai transformar em uma representação interna que ele entende, normalmente em um tipo de "árvore", e só então irá começar a executar as instruções passadas. Quando terminar o seu programa, o interpretador também terminará.*

---
*Assim funcionam linguagens como **Perl**, **Php**, **Python**, **Ruby** e até **Javascript**. Elas variam em algumas funcionalidades, por exemplo: Perl e Python permitem pré-compilar seu código-'fonte, na representação intermediaria falada anteriormente.*