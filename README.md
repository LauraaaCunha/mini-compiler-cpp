# Mini Compilador (C++)

Projeto da disciplina de Compiladores (IFRS - Campus Ibirubá).
Implementa as duas primeiras fases de um compilador para uma linguagem
simples de comandos de movimento:

- **Análise léxica** (`lexer.cpp`): transforma o texto em tokens.
- **Análise sintática** (`parser.cpp`): verifica se os tokens seguem a gramática.

## Linguagem

Todo programa começa com `inicio` e termina com `fim`.
Comandos: `andar N;` `virar direita|esquerda;` `esperar N;` `parar N;` `desviar N;`

Exemplo:
inicio desviar 5; parar 1; esperar 2; andar 10; fim

## Como compilar e executar

g++ -std=c++17 aula6.cpp lexer.cpp parser.cpp -o aula6
./aula6        (no Windows: .\aula6.exe)

O programa lê o código em uma única linha.
