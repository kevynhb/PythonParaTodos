# Estudos livro Python para todos 

Estudos do livro python para todos do autor: Charles R. Severance

// Anotando conhecimentos/ideias que preciso fixar mais na memória.
// Material para consulta, reler conceitos.


# Explorando Dados com Python 3

**Entrada (input)** - entrada de dados do ‘mundo externo’ no sistema, como arquivos, sensores, microfone, GPS e etc…

**Saída (output)** - mostrar resultados em tela, ou guardá-los em um arquivo.

---

### **Erros de Sintaxe:**

Estes são os primeiros erros que você vai cometer e os mais
fáceis para corrigir. Um erro de sintaxe significa que você violou as regras da “gramática” do Python.

### **Erros de Lógica:**

Um erro lógico é quando o programa tem uma boa sintaxe, mas há um erro na ordem das afirmações ou talvez um erro na forma como as afirmações se relacionam entre si. UM bom exemplo de um erro lógico pode ser, “abra sua garrafa e beba um pouco d’água, coloque-a em sua mochila, caminhe até a biblioteca e, somente em seguida, tampe a garrafa.”

### **Erros de Semântica:**

Um erro semântico é quando a descrição dos passos a serem
tomados é sintaticamente perfeita e na ordem certa, mas há um erro no programa. Ele está perfeito, mas não faz o que você pretendia que fizesse. Um exemplo simples seria se você estivesse dando a uma pessoa direções para um restaurante e dissesse: “. . . quando você chegar no cruzamento com o posto
de gasolina, vire à esquerda e vá um quilômetro de distância e o restaurante é um edifício vermelho à sua esquerda.” Seu amigo está muito atrasado e te liga para dizer que eles estão em uma fazenda, andando por trás de um celeiro, sem sinal de um restaurante. Então você diz “você virou à esquerda ou direita o posto de gasolina?” e Ele diz, “Eu segui suas direções perfeitamente, eu as escrevi todas: diz para virar à esquerda e seguir um quilômetro em direção ao posto de gasolina.” Então
você diz, “Eu sinto muito, porque enquanto minhas instruções foram sintaticamente corretas, elas infelizmente continham um erro semântico pequeno, mas não detectado.”

---

Novamente em todos os três tipos de erros, Python está tentando ao máximo apenas fazer exatamente o que você pediu.

## Debugging

**Ler** Leia seu código. Fale-o em voz alta para si próprio e verifique se ele diz mesmo o que você quer que ele diga.

**Testar** Experimente fazer mudanças e rodar diferentes versões do seu programa. Geralmente, quando você coloca a coisa certa no lugar certo, o problema se torna óbvio, porém, às vezes, você precisará levar um tempo para encontrar o que deve ser ajustado.

**Refletir** Tire um tempo para pensar! Que tipo de erro está acontecendo: sintaxe, semântica, em tempo de execução? Que informações você pode extrair das mensagens de erro, ou da saída do programa? Que tipo de erro poderia causar o problema que você está vendo? Qual foi a última coisa que você alterou antes do problema aparecer? 

**Retroceder** Em certo momento, o melhor a se fazer é voltar atrás. Desfazer mudanças recentes, até retornar a um programa que funcione e que você o entenda. Depois você pode começar a reconstruir o código.

---

### Glossário

**erro de semântica:** Um erro em um programa que faz com que, na execução, ele faça algo diferente do que o programador intencionou.

**Compilar:** Ação de traduzir um programa escrito em uma linguagem de alto nível em uma linguagem de baixo nível, tudo em preparação, para a execução posterior.

**interpretar:** Executar um programa em uma linguagem de alto nível, traduzindo-o uma linha por vez.

**programa:** Um conjunto de instruções que especifica a computação a ser executada pela máquina.

**semântica:** O significado de um programa.

[1.14 Exercícios](https://www.notion.so/1-14-Exerc-cios-00347eae92604b8580c308330c280859)

# Cap02 - Variáveis, expressões e declarações

### Tipo

Quando você digita um inteiro muito grande, você deve estar tentado a usar uma
vírgula entre grupos de três dígitos 1,000,000. Isso não é um inteiro válido em
Python, mas é válido:

> print(1,000,000)
1 0 0
> 

Bom, não é o que esperávamos! Python interpreta **1,000,000** como uma sequência de inteiros separada por vírgulas, a qual é mostrada com um espaço entre cada inteiro.

**index{erro semântico}**

Esse é o primeiro exemplo em que vemos um erro semântico: o código é executado sem mostrar nenhuma mensagem de erro, mas não faz a coisa “certa”.

## Variáveis

Uma variável é um nome que faz referência a um valor.

> **message** = 'E agora, para algo completamente diferente'
**n** = ****17
**pi** = 3.1415926535897931
> 

Valores atribuídos as variáveis.

### Python reserva 33 palavras-chave para o seu uso:

**and -** e
**as -** como
**assert -** afirmar
**break -** parar
**class -** Classe
**continue -** Prosseguir
**def 
del
elif
else -** senão
**except -** exceto
**False
finally -** finalmente
**for -** por
**from -** a partir de
**global 
if -** e se
**import -** import

**in -** dentro
**is -** é
**lambda 
None -** nenhum
**nonlocal -** não local
**not -** não
**or -** ou 
**pass -** passar
**raise -** levantar
**return -** retorna
**True -** verdadeiro
**try -** tentar
**while -** enquanto
**with -** com 
**yield -** colheita

---

### Operadores e Operandos

Operadores são símbolos especiais que representam operações como adição e multiplicação. Os valores em que o operador é aplicado são chamados **operandos**.

Os operadores **+, -, *, /, e **** realizam respectivamente adição, subtração, multiplicação, divisão, e exponenciação, como nos seguintes exemplos:*333

20+32
hora-1
hora*60+minuto
minuto/60
5**2
(5+9)*(15-7)

Resposta em Python 3.x use a divisão inteira(//inteiro).
minute = 59
minute//60
0

Em Python 3.x a divisão de números inteiros funciona de maneira muito mais semelhante ao que você esperaria se colocasse a expressão em uma calculadora.

### Expressões

Uma **expressão** é uma combinação de valores, variáveis e operandos. um valor por si só, é considerado uma expressão, assim como uma variável.
