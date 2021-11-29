# ciscoPythonCourse
Notas curso Python de Cisco

print() funcion(argumento) muestra cadenas ente aspas '' o ""

Que argumentos print() espera?

Quaisquer. Mostrar-lhe-emos em breve que print() é capaz de operar com virtualmente todos os tipos de dados oferecidos pelo Python. Strings, números, carateres, valores lógicos, objetos - qualquer um destes pode ser passado com sucesso para print().

Simbolo de escape con n para agregar un salto de linea  /n
 para usar varios argumentos en una funcion se separan los argumentos con , virgula
 
 
    a função print() invocada com mais do que um argumento faz output de todos eles numa só linha;
    a função print() coloca um espaço entre os argumentos de output, por sua própria iniciativa.

forma posicional de passar argumentos
argumentos de keyword  ej. end = " "  (indica como se representará el final de la funcion, por omision es equivalente a end = "/n")
 O argumento de keyword que pode fazer isto é chamado sep (como separador)
 print("My", "name", "is", "Monty", "Python.", sep="-")
 
 print("My", "name", "is", sep="_", end="*")
print("Monty", "Python.", sep="*", end="*\n")


 2.1.1.18 LAB: A função print()


Tempo estimado

5-10 minutos
Nível de dificuldade

Muito fácil
Objetivos

    familiarizar-se com a função print() e as suas capacidades de formatação;
    experimentar com código Python.

Cenário

Modifique a primeira linha de código no editor, usando as keywords sep e end , para corresponder ao output esperado. Use as duas print() funções no editor.

Não mude nada na segunda invocação print() .
Output esperado
Programming***Essentials***in...Python

Solucion
print("Programming","Essentials","in", sep="***", end="...")
print("Python")

 2.1.1.19 LAB: Formatar o output
LAB

Tempo estimado

5-15 minutos
Nível de dificuldade

Fácil
Objetivos

    experimentar com o código Python existente;
    descobrir e corrigir erros básicos de sintaxe;
    familiarizar-se com a função print() e os seus recursos de formatação.

Cenário

Encorajamo-lo vivamente a brincar com o código que escrevemos para si, e a fazer algumas (talvez mesmo destrutivas) alterações. Sinta-se livre para modificar qualquer parte do código, mas há uma condição - aprenda com os seus erros e tire as suas próprias conclusões.

Tente:

    minimizar o número de invocações da função print() inserindo a sequência \n nas strings
    fazer a seta duas vezes maior (mas mantendo as proporções)
    duplicar a seta, colocando ambas as setas lado a lado; nota: uma string pode ser multiplicada usando o seguinte truque: "string" * 2 produzirá "stringstring" (brevemente, falaremos mais sobre o assunto)
    retire qualquer uma das aspas, e veja cuidadosamente a resposta do Python; preste atenção ao local onde o Python vê um erro - é este o local onde o erro realmente existe?
    faça o mesmo com alguns dos parêntesis;
    altere qualquer uma das print palavras por outra coisa, diferindo apenas no caso (por exemplo, Print) - o que acontece agora?
    substitua algumas das aspas por apóstrofes; observe cuidadosamente o que acontece.

print("    *")
print("   * *")
print("  *   *")
print(" *     *")
print("***   ***")
print("  *   *")
print("  *   *")
print("  *****")

https://edube.org/sandbox/bb018eb8-4e38-11ec-af5b-0242157e55ca
https://edube.org/sandbox/cedee96c-4e38-11ec-9033-0242157e55ca

Key takeaways

1. A função print() é uma função incorporada. Imprime/faz output de uma mensagem especificada para a janela do ecrã/consola.

2. As funções incorporadas, ao contrário das funções definidas pelo utilizador, estão sempre disponíveis e não têm de ser importadas. O Python 3.8 vem com 69 funções incorporadas. Pode encontrar a sua lista completa fornecida em ordem alfabética na Biblioteca Padrão Python.

3. Para chamar uma função (este processo é conhecido como invocação de função ou chamada de função), é necessário usar o nome da função seguido de parêntesis. Pode passar argumentos para uma função, colocando-os dentro dos parêntesis. Deve separar os argumentos com uma vírgula, por exemplo, print("Hello,", "world!"). Uma função “vazia” print() faz output de uma linha vazia para o ecrã.

4. As strings de Python são delimitadas com aspas, por exemplo, "I am a string" (aspas duplas), ou 'I am a string, too' (aspas simples).

5. Os programas de computador são coleções de instruções. Uma instrução é um comando para executar uma tarefa específica quando executada, por exemplo, para imprimir uma determinada mensagem no ecrã.

6. Em strings de Python a barra invertida (\) é um caratere especial que anuncia que o próximo caratere tem um significado diferente, por exemplo \n (the newline character) starts a new output line.

7. Os argumentos posicionais são aqueles cujo significado é ditado pela sua posição, por exemplo, o segundo argumento é apresentado após o primeiro, o terceiro é apresentado após o segundo, etc.

8. Os argumentos de keyword são aqueles cujo significado não é ditado pela sua localização, mas por uma palavra especial (keyword) utilizada para os identificar.

9. Os loops end e sep podem ser usados para formatar o output da função print() . O parâmetro sep especifica o separador entre os argumentos de output (por exemplo, o parâmetro print("H", "E", "L", "L", "O", sep="-"), enquanto o parâmetro end especifica o que imprimir no final da declaração print.

Literales o tipos de datos en Python
En enteros se pueden usar underscores para separar las unidades de mil. Ej: 11_111_111
Se usa 0o para especificar si un numero es octal y 0x para los numeros hexadecimales

Los float usan el punto decimal como separador de su parte fracionaria
sa debe usar 3E8 o 3e8 para indicar un exponente decimal
1e-22
Strings
Se pueden incluir aspas en un string usando el caracter se escape /" o intercalando dobles comillas con sencillas
print('I\'m Monty Python.')
print("I'm Monty Python.")
Booleanos estan determinados por los vaslores True y False
print(True > False)
print(True < False)



2.2.1.11 LAB: literais de Python - strings
Tempo estimado

5-10 minutos
Nível de dificuldade

Fácil
Objetivos

    familiarizar-se com a função print() e as suas capacidades de formatação;
    praticar codificação de strings;
    experimentar com código Python.

Cenário

Escreva um código de uma linha, utilizando a função print() , bem como os carateres de newline e de escape, para corresponder ao resultado esperado emitido em três linhas.
Output esperado

"I'm"
""learning""
"""Python"""

Solucion
print('"I\'m"\n','""learning""\n','"""Python"""', sep="")

Key takeaways

1. Os literais são notações para representar alguns valores fixos em código. O Python tem vários tipos de literais - por exemplo, um literal pode ser um número (literais numéricos, por exemplo, 123), ou uma string (literais de string, por exemplo, “Eu sou um literal.“).

2. O sistema binário é um sistema de números que emprega 2 como base. Portanto, um número binário é composto apenas por 0s e 1s, por exemplo, 1010 é 10 em decimal.
Os sistemas de numeração octal e hexadecimal, do mesmo modo, empregam 8 e 16 como suas bases, respetivamente. O sistema hexadecimal utiliza os números decimais e seis letras extra.

3. Inteiros (ou simplesmente ints) são um dos tipos numéricos suportados pelo Python. São números escritos sem um componente fracionário, por exemplo, 256, ou -1 (inteiros negativos).

4. Números de floating-point (ou simplesmente floats) são outro dos tipos numéricos suportados pelo Python. São números que contêm (ou são capazes de conter) um componente fracionário, por exemplo 1.27.

5. Para codificar uma apóstrofe ou uma aspa dentro de uma string, pode usar o caratere de escape, por exemplo, 'I\'m happy.', ou abrir e fechar a string utilizando um conjunto de símbolos opostos aos que deseja codificar, por exemplo "I'm happy." codificar uma apóstrofe, e 'He said "Python", not "typhoon"' para codificar umas aspas (duplas).

6. Valores booleanos são os dois objetos constantes True e False usado para representar valores de verdade (em contextos numéricos 1 é True, enquanto 0 é False.

EXTRA

Há mais um literal especial que é usado em Python: o literal None . Este literal é um chamado NoneType objeto, e é utilizado para representar a ausência de um valor. Em breve, contar-lhe-emos mais sobre isso.

Operadores matematicos
Começaremos pelos operadores que estão associados às operações aritméticas mais amplamente reconhecidas:

+, -, *, /, //, %, **

É possível formular as seguintes regras com base neste resultado:

    quando ambos os argumentos ** são inteiros, o resultado é também um inteiro;
    quando pelo menos um argumento ** é um float, o resultado é também um float.
print(2 ** 3)
print(2 ** 3.)
print(2. ** 3)
print(2. ** 3.)

O resultado produzido pelo operador da divisão é sempre um float
print(6 / 3)
print(6 / 3.)
print(6. / 3)
print(6. / 3.)

O resultado da divisão inteira é sempre arredondado para o valor inteiro mais próximo, que é inferior ao resultado real (não arredondado).

Isto é muito importante: o arredondamento vai sempre para o número inteiro menor.
Modulo (%) O resultado do operador é um remainder (resto) deixado após a divisão inteira.
operadores unarios y binarios

La prioridad de operaciones es de izquierda a derecha con excepcion de la exponenciacion que va de derecha a izquierda


Prioridade 	Operador 	
1 	+, - 	unário
2 	** 	
3 	*, /, //, % 	
4 	+, - 	binário

Key takeaways

1. Uma expressão é uma combinação de valores (ou variáveis, operadores, chamadas a funções - em breve aprenderá sobre elas) que avalia a um valor, por exemplo, 1 + 2.

2. Os operadores são símbolos especiais ou keywords capazes de operar sobre os valores e realizar operações (matemáticas), por exemplo, o * operador multiplica dois valores: x * y.

3. Operadores aritméticos em Python: + (adição), - (subtração), * (multiplicação), / (divisão clássica - devolve sempre um float), % (módulo - divide o operando esquerdo pelo operando direito e devolve o resto da operação, por exemplo, 5 % 2 = 1), ** (exponenciação - operando esquerdo elevado à potência do operando direito, por exemplo, 2 ** 3 = 2 * 2 * 2 = 8), // (divisão por piso/inteiro - devolve um número resultante da divisão, mas arredondado para baixo para o número inteiro mais próximo, por exemplo 3 // 2.0 = 1.0)

4. Um operador unário é um operador com apenas um operando, por exemplo, -1, ou +3.

5. Um operador binário é um operador com dois operandos, por exemplo, 4 + 5, ou 12 % 5.

6. Alguns operadores atuam antes de outros - a hierarquia de prioridades:

    unário + e - têm a prioridade mais alta
    depois: **, depois: *, /, e %e, depois, a prioridade mais baixa: binário + e -.

7. Subexpressões entre parêntesis são sempre calculadas em primeiro lugar, por exemplo, 15 - 1 * (5 * (1 + 2)) = 0.

8. O operador de exponenciação utiliza ligação do lado direito, por exemplo 2 ** 2 ** 3 = 256.


¿Qué son las Variables?

Es justo que Python nos permita codificar literales, las cuales contengan valores numéricos y cadenas.

Ya hemos visto que se pueden hacer operaciones aritméticas con estos números: sumar, restar, etc. Esto se hará una infinidad de veces en un programa.

Pero es normal preguntar como es que se pueden almacenar los resultados de estas operaciones, para poder emplearlos en otras operaciones, y así sucesivamente.

¿Cómo almacenar los resultados intermedios, y después utilizarlos de nuevo para producir resultados subsecuentes?

Python ayudará con ello. Python ofrece "cajas" (contenedores) especiales para este propósito, estas cajas son llamadas variables - el nombre mismo sugiere que el contenido de estos contenedores puede variar en casi cualquier forma.

¿Cuáles son los componentes o elementos de una variable en Python?

    Un nombre.
    Un valor (el contenido del contenedor).

Comencemos con lo relacionado al nombre de la variable.

Las variables no aparecen en un programa automáticamente. Como desarrollador, tu debes decidir cuantas variables deseas utilizar en tu programa.

También las debes de nombrar.

Si se desea nombrar una variable, se deben seguir las siguientes reglas:

    El nombre de la variable debe de estar compuesto por MAYUSCULAS, minúsculas, dígitos, y el carácter _ (guion bajo).
    El nombre de la variable debe comenzar con una letra.
    El carácter guion bajo es considerado una letra.
    Las mayúsculas y minúsculas se tratan de forma distinta (un poco diferente que en el mundo real - Alicia y ALICIA son el mismo nombre, pero en Python son dos nombres de variable distintos, subsecuentemente, son dos variables diferentes).
    El nombre de las variables no pueden ser igual a alguna de las palabras reservadas de Python (se explicará más de esto pronto).


O que são variáveis?

Parece bastante óbvio que o Python deveria permitir-lhe codificar literais transportando valores de número e texto.

Já sabe que pode fazer algumas operações aritméticas com estes números: adicionar, subtrair, etc. Fá-lo-á muitas vezes.

Mas é uma questão bastante normal de perguntar como armazenar os resultados destas operações, a fim de os utilizar noutras operações, e assim por diante.

Como guardar os resultados intermediários, e utilizá-los novamente para produzir os resultados subsequentes?

O Python irá ajudá-lo nisso. Oferece "caixas" especiais (em inglês, containers) para esse fim, e estas caixas são chamadas variáveis - o próprio nome sugere que o conteúdo destes containers pode ser variado em (quase) qualquer forma.

O que tem cada variável Python?

    um nome;
    um valor (o conteúdo do container)

Comecemos com as questões relacionadas com o nome de uma variável.

As variáveis não aparecem automaticamente num programa. Como programador, deve decidir quantas e quais as variáveis a utilizar nos seus programas.

Deve também nomeá-las.

Se quiser dar um nome a uma variável, deve seguir algumas regras estritas:

    o nome da variável deve ser composto por letras maiúsculas ou minúsculas, dígitos e o caratere _ (underscore)
    o nome da variável deve começar com uma letra;
    o caratere underscore é uma letra;
    letras maiúsculas e minúsculas são tratadas como diferentes (um pouco diferente do que no mundo real - Alice e ALICE são os mesmos nomes próprios, mas em Python são dois nomes de variáveis diferentes, e consequentemente, duas variáveis diferentes);
    o nome da variável não deve ser nenhuma das palavras reservadas de Python (as keywords - explicaremos mais sobre isto em breve).

Uma variável passa a existir como o resultado da atribuição de um valor a ela. Ao contrário de outras linguagens, não precisa de a declarar de nenhuma forma especial.

Pode utilizar a função print() e combinar texto e variáveis usando o operador + para fazer output de strings e variáveis, por exemplo:
var = "3.8.5"
print("Python version: " + var)

2.4.1.7 LAB: Variáveis


TRabajo perdido
LAB
john = 3
mary = 5
adam = 6
print(john,mary,adam, sep=",")
totalApples = john + mary + adam
print(totalApples)
print("Total number of apples: ",totalApples)
FIN LAB

Operadores Abreviados

Es tiempo de explicar el siguiente conjunto de operadores que harán la vida del programador/desarrollador mas fácil.

Muy seguido, se desea utilizar la misma variable al lado derecho y al lado izquierdo del operador =.

Por ejemplo, si se necesita calcular una serie de valores sucesivos de la potencia de 2, se puede usar el siguiente código:
x = x * 2

También, puedes utilizar una expresión como la siguiente si no puedes dormir y estas tratando de resolverlo con alguno de los métodos tradicionales:
oveja = oveja + 1

Python ofrece una manera mas corta de escribir operaciones como estas, lo cual se puede codificar de la siguiente manera:
x *= 2
oveja+= 1

A continuación se intenta presentar una descripción general para este tipo de operaciones.

Si op es un operador de dos argumentos (esta es una condición muy imporante) y el operador es utilizado en el siguiente contexto:
variable = variable op expresión

Puede ser simplificado de la siguiente manera:
variable op= expresión

Observa los siguientes ejemplos. Asegúrate de entenderlos todos.

i = i + 2 * j ⇒ i += 2 * j

var = var / 2 ⇒ var /= 2

rem = rem % 10 ⇒ rem %= 10

j = j - (i + var + rem) ⇒ j -= (i + var + rem)

x = x ** 2 ⇒ x **= 2


Shortcuts operators
Let's try to present a general description for these operations.

If op is a two-argument operator (this is a very important condition) and the operator is used in the following context:
variable = variable op expression

It can be simplified and shown as follows:
variable op= expression

Take a look at the examples below. Make sure you understand them all.

i = i + 2 * j ⇒ i += 2 * j

var = var / 2 ⇒ var /= 2

rem = rem % 10 ⇒ rem %= 10

j = j - (i + var + rem) ⇒ j -= (i + var + rem)

x = x ** 2 ⇒ x **= 2

Sin corregir:
kilometros = 12.25
millas = 7.38

millas_a_kilometros = ###
kilometros_a_millas = ###

print(millas, " millas son ", round(millas_a_kilometros, 2), " kilómetros ")
print(kilometros, " kilómetros son ", round(kilometros_a_millas, 2), " millas ")

LAB
kilometers = 12.25
miles = 7.38

miles_to_kilometers = miles * (1.61)
kilometers_to_miles = kilometers / (1.61)

print(miles, "miles is", round(miles_to_kilometers, 2), "kilometers")
print(kilometers, "kilometers is", round(kilometers_to_miles, 2), "miles")
FIN LAB
round(arg1,arg2) Funcion redondeo a muneros decimales indicados en arg2 

LAB
x =  -1
x = float(x)
y = (3 * x ** 3) - (2 * x ** 2) + (3 * x) - 1
print("y =", y)
FIN LAB

Key takeaways

1. Uma variável é um local nomeado, reservado para armazenar valores na memória. Uma variável é criada ou inicializada automaticamente quando se lhe atribui um valor pela primeira vez. (2.1.4.1)

2. Cada variável deve ter um nome exclusivo - um identificador. Um nome de identificador válido deve ser uma sequência não vazia de carateres, deve começar com o underscore (_), ou uma letra, e não pode ser uma keyword de Python. O primeiro caratere pode ser seguido por underscores, letras e dígitos. Os identificadores em Python diferenciam entre maiúsculas e minúsculas (são case-sensitive). (2.1.4.1)

3. O Python é uma linguagem dinamicamente dactilografada, o que significa que não precisa de declarar variáveis nela contidas. (2.1.4.3) Para atribuir valores a variáveis, pode-se utilizar um operador de atribuição simples na forma do sinal (=) igual, ou seja, var = 1.

4. Também pode utilizar operadores de atribuição composta (operadores de atalho) para modificar valores atribuídos a variáveis, por exemplo, var += 1, ou var /= 5 * 2. (2.1.4.8)

5. Pode atribuir novos valores a variáveis já existentes, utilizando o operador de atribuição ou um dos operadores compostos, por exemplo: (2.1.4.5)
var = 2
print(var)

var = 3
print(var)

var += 1
print(var)


6. Pode combinar texto e variáveis utilizando o operador + , e utilizar a função print() para fazer output de strings e variáveis, por exemplo: (2.1.4.4)
var = "007"
print("Agent " + var)


The comment are made with the # symbol
2.1.5.2 LABORATORIO: Comentarios
LAB
#this program computes the number of seconds in a given number of hours
# this program has been written two days ago

a = 2 # number of hours
seconds = 3600 # number of seconds in 1 hour

print("Hours: ", a) 
print("Seconds in Hours: ", a * seconds) # printing the number of seconds in a given number of hours
print("Goodbye")
#here we should also print "Goodbye", but a programmer didn't have time to write any code
#this is the end of the program that computes the number of seconds in 2 hour
FIN LAB
#this program computes the number of seconds in a given number of hours

hours = 2 
seconds = 3600 # number of seconds in 1 hour

print("Hours: ", hours) #printing the number of hours
print("Seconds in Hours: ", hours * seconds) # printing the number of seconds in a given number of hours
print("Goodbye")

Key takeaways

1. Os comentários podem ser utilizados para deixar informações adicionais em código. São omitidos em runtime. A informação deixada no source code é dirigida aos leitores humanos. Em Python, um comentário é um pedaço de texto que começa com #. O comentário estende-se até ao fim da linha.

2. Se quiser colocar um comentário que abranja várias linhas, precisa de colocar # à frente de todas elas. Além disso, pode utilizar um comentário para marcar um pedaço de código que não é necessário neste momento (ver a última linha do snippet abaixo), por exemplo:
# This program prints
# an introduction to the screen.
print("Hello!")  # Invoking the print() function
# print("I'm Python.")


3. Sempre que possível e justificado, deve dar nomes self-commenting às variáveis, por exemplo, se estiver a utilizar duas variáveis para armazenar um comprimento (em inglês, length) e largura (width) de algo, os nomes das variáveis length e width podem ser uma escolha melhor do que myvar1 e myvar2.

4. É importante utilizar comentários para tornar os programas mais fáceis de compreender, e utilizar nomes de variáveis legíveis e significativos em código. Contudo, é igualmente importante não usar nomes de variáveis que sejam confusos, ou deixar comentários que contenham informações erradas ou incorretas!

5. Os comentários podem ser importantes quando você estiver a ler o seu próprio código após algum tempo (confie em nós, os programadores esquecem-se do que o seu próprio código faz), e quando outros estão a ler o seu código (pode ajudá-los a compreender o que os seus programas fazem e como o fazem mais rapidamente).

Puntos Clave

1. Los comentarios pueden ser utilizados para colocar información adicional en el código. Son omitidos al momento de la ejecución. Dicha información es para los lectores que están manipulando el código. En Python, un comentario es un fragmento de texto que comienza con un #. El comentario se extiende hasta el final de la línea.

2. Si deseas colocar un comentario que abarque varias líneas, es necesario colocar un # al inicio de cada línea. Además, se puede utilizar un comentario para marcar un fragmento de código que no es necesaria en el momento y no se desea ejecutar. (observa la ultima línea de código del siguiente fragmento), por ejemplo:
# Este programa imprime
# un saludo en pantalla
print("Hola!")  # Se invoca la función print() function
# print("Soy Python.")

3. Cuando sea posible, se deben auto comentar los nombres de las variables, por ejemplo, si se están utilizando dos variables para almacenar la altura y longitud de algo, los nombres altura y longitud son una mejor elección que mivar1 y mivar2.

4. Es importante utilizar los comentarios para que los programas sean más fáciles de entender, además de emplear variables legibles y significativas en el código. Sin embargo, es igualmente importante no utilizar nombres de variables que sean confusos, o dejar comentarios que contengan información incorrecta.

5. Los comentarios pueden ser muy útiles cuando tu estas leyendo tu propio código después de un tiempo (es común que los desarrolladores olviden lo que su propio código hace), y cuando otros están leyendo tu código (les puede ayudar a comprender que es lo que hacen tus programas y como es que lo hacen).


Já o dissemos, mas deve ser afirmado uma vez mais sem ambiguidade: o resultado da função input() é uma string.

input() function supports arguments and captures strings
input("Esta pregunta aparece sin problema: ")

Type casting
Las funciones int() y float() sirven para cambiar el tipo de dato ingresado

e.g. 
anything = float(input("Enter a number: "))
something = anything ** 2.0
print(anything, "to the power of 2 is", something)

leg_a = float(input("Input first leg length: "))
leg_b = float(input("Input second leg length: "))
hypo = (leg_a**2 + leg_b**2) ** .5
print("Hypotenuse length is", hypo)

leg_a = float(input("Input first leg length: "))
leg_b = float(input("Input second leg length: "))
print("Hypotenuse length is", (leg_a**2 + leg_b**2) ** .5)



Concatenation uses + 

Replication uses * to reply strings

print("+" + 10 * "-" + "+")
print(("|" + " " * 10 + "|\n") * 5, end="")
print("+" + 10 * "-" + "+")

Type cast con str() function

leg_a = float(input("Input first leg length: "))
leg_b = float(input("Input second leg length: "))
print("Hypotenuse length is " + str((leg_a**2 + leg_b**2) ** .5))

LAB
# input a float value for variable a here
a = float(input("Ingrese valor a: "))
# input a float value for variable b here
b = float(input("Ingrese valor b: "))
# output the result of addition here
print("La suma de los dos numeros es:", a + b)
# output the result of subtraction here
print("La resta de los dos numeros es:", a - b)
# output the result of multiplication here
print("El pŕoducto de los dos numeros es:", a * b)
# output the result of division here
print("La division de los dos numeros es:", a / b)

print("\nThat's all, folks!")
FIN LAB


 2.6.1.10 LAB: Operadores e expressões
Tempo estimado

20 minutos
Nível de dificuldade

Intermédio
Objetivos

    familiarizar-se com o conceito de números, operadores e operações aritméticas em Python;
    compreender a precedência e associatividade dos operadores Python, bem como o uso adequado de parêntesis.

Cenário

A sua tarefa é a de completar o código, de forma a avaliar a seguinte expressão:

O resultado deve ser atribuído a y. Tenha cuidado - observe os operadores e mantenha as suas prioridades em mente. Não hesite em utilizar os parêntesis de que necessitar.

Pode utilizar variáveis adicionais para encurtar a expressão (mas não é necessário). Teste o seu código com cuidado.

Dados de Teste

Input de amostra: 1

Output esperado:
y = 0.6000000000000001

Input de amostra: 10

Output esperado:
y = 0.09901951266867294

Input de amostra: 100

Output esperado:
y = 0.009999000199950014

Input de amostra: -5

Output esperado:
y = -0.19258202567760344

    Sandbox

Code
x = float(input("Enter value for x: "))

# Write your code here.

print("y =", y)

    Console


****

**Nível de dificuldade

Fácil
Objetivos

    melhorar a capacidade de utilizar números, operadores, e operações aritméticas em Python;
    utilizar as capacidades de formatação da função print() ;
    aprender a expressar os fenómenos da vida quotidiana em termos de linguagem de programação.

Cenário

A sua tarefa é preparar um código simples capaz de avaliar o tempo final de um período de tempo, dado como um número de minutos (pode ser arbitrariamente grande). O tempo inicial é dado como um par de horas (0.. 23) e minutos (0.. 59). O resultado tem de ser impresso para a consola.

Por exemplo, se um evento começar às 12:17 e durar 59 minutos, ele terminará às 13:16.

Não se preocupe com quaisquer imperfeições no seu código - não faz mal se aceitar um tempo inválido - o mais importante é que o código produza resultados válidos para dados de input válidos.

Teste o seu código com cuidado. Dica: utilizar o operador % pode ser a chave para o sucesso.
Dados de teste

Input de amostra:
12
17
59

Output esperado: 13:16

Input de amostra:
23
58
642


Output esperado: 10🈴**


x = float(input("Enter value for x: "))
y = 1./(x + 1./(x + 1./(x + 1./x)))
print("y =", y)

hour = int(input("Starting time (hours): "))
mins = int(input("Starting time (minutes): "))
dura = int(input("Event duration (minutes): "))

# put your code here
added_hour = dura / 60
added_mins = dura % 60
final_hour = hour + added_hour
final_mins = mins + added_mins


print(round(final_hour), final_mins, sep = ":")

Key takeaways

1. A função print() envia dados para a consola, enquanto a função input() obtém dados da consola.

2. O método input() vem com um parâmetro opcional: a string prompt. Permite-lhe escrever uma mensagem antes do input do utilizador, por exemplo
name = input("Enter your name: ")
print("Hello, " + name + ". Nice to meet you!")


3. Quando a função input() é chamada, o fluxo do programa é interrompido, o símbolo de prompt continua a piscar (pede ao utilizador para tomar medidas quando a consola é mudada para o modo de input) até o utilizador ter introduzido um input e/ou premido a tecla Enter.

NOTA

Pode testar a funcionalidade da função input() em todo o seu scope localmente na sua máquina. Por razões de otimização de recursos, limitámos o tempo máximo de execução do programa no Edube a alguns segundos. Vá à Sandbox, copie-cole o snippet acima, execute o programa, e não faça nada - espere apenas alguns segundos para ver o que acontece. O seu programa deve ser interrompido automaticamente após um breve momento. Agora abra o IDLE, e execute lá o mesmo programa - consegue ver a diferença?

Dica: a característica acima mencionada da função input() pode ser utilizada para solicitar o utilizador a terminar um programa. Veja o código em baixo:
name = input("Enter your name: ")
print("Hello, " + name + ". Nice to meet you!")

print("\nPress Enter to end the program.")
input()
print("THE END.")


3. O resultado da função input() é uma string. Podem adicionar-se strings umas às outras usando a concatenação (+) operador. Verifique este código:
num_1 = input("Enter the first number: ") # Enter 12
num_2 = input("Enter the second number: ") # Enter 21

print(num_1 + num_2) # the program returns 1221


4. Também pode multiplicar (* - replicação) strings, por exemplo:
my_input = input("Enter something: ") # Example input: hello
print(my_input * 3) # Expected output: hellohellohello





Modulo 3
Comparison operators
== ¡= > >= < <= 

Priority 	Operator 	
1 	+, - 	unary
2 	** 	
3 	*, /, //, % 	
4 	+, - 	binary
5 	<, <=, >, >= 	
6 	==, !=

if true_or_not:
    do_this_if_true
    
if true_or_false_condition:
    perform_if_condition_true
else:
    perform_if_condition_false
    
if the_weather_is_good
    go_for_a_walk()
elif tickets_are_available:
    go_to_the_theater()
elif table_is_available:
    go_for_lunch()
else:
    play_chess_at_home()

max() maximo numero de varios argumentos
min() minimo numero de varios argumentos
LAB
text = input("Write your favorite plant: ")
if text == "Spathiphyllum":
    print("Yes - Spathiphyllum is the best plant ever!")
else:
    if text == "spathiphyllum":
        print("No, I want a big Spathiphyllum!")
    else:
        print("Spathiphyllum! Not " + text + "!")
    
 END LAB
 tax = round(tax, 0)
 
 LAB
 
income = float(input("Enter the annual income: "))

if income < 85528:
   tax =  (income * 0.18) - 556.2
else:
    if income > 85528:
        tax = 14839.2 + ((income - 85528) * 0.32)
if tax <= 0:
    tax = 0.0

tax = round(tax, 0)
print("The tax is:", tax, "thalers")
END LAB

LAB


 year = int(input("Enter a year: "))
if year < 1582:
    print("Not within the Gregorian calendar period")
else:
    if (year % 4) != 0:
        print("Common year")
    elif (year % 100) != 0:
        print("Leap year")
    elif (year % 400) != 0:
        print("Common year")
    else:
        print("Leap year")
 END LAB
 
 x = 10

if x == 10: # True
    print("x == 10")

if x > 15: # False
    print("x > 15")

elif x > 10: # False
    print("x > 10")

elif x > 5: # True
    print("x > 5")

else:
    print("else will not be executed")
    
 Otro ejemplo de condicionales indentados
 
 x = 10

if x > 5: # True
    if x == 6: # False
        print("nested: x == 6")
    elif x == 10: # True
        print("nested: x == 10")
    else:
        print("nested: else")
else:
    print("else")
    
 LOOPS
 
 while conditional_expression:
    instruction
    
 counter = 5
while counter != 0:
    print("Inside the loop.", counter)
    counter -= 1
print("Outside the loop.", counter)

# A program that reads a sequence of numbers
# and counts how many numbers are even and how many are odd.
# The program terminates when zero is entered.

odd_numbers = 0
even_numbers = 0

# Read the first number.
number = int(input("Enter a number or type 0 to stop: "))

# 0 terminates execution.
while number != 0:
    # Check if the number is odd.
    if number % 2 == 1:
        # Increase the odd_numbers counter.
        odd_numbers += 1
    else:
        # Increase the even_numbers counter.
        even_numbers += 1
    # Read the next number.
    number = int(input("Enter a number or type 0 to stop: "))

# Print results.
print("Odd numbers count:", odd_numbers)
print("Even numbers count:", even_numbers)


 3.1.2.3 LABORATORIO: Lo esencial del ciclo while - Adivina el número secreto

LAB

secret_number = 777

print(
"""
+================================+
| Welcome to my game, muggle!    |
| Enter an integer number        |
| and guess what number I've     |
| picked for you.                |
| So, what is the secret number? |
+================================+
""")

guessing = int(input("Type a number, please: "))
while guessing != secret_number:
    print("Ha ha! You're stuck in my loop!")
    guessing = int(input("Type a number, please: "))
print(secret_number)
print("Well done, muggle! You are free now.")

END LAB


Fazer loop ao seu código com for

Outro tipo de loop disponível em Python vem da observação de que por vezes é mais importante contar as "voltas" do loop do que verificar as condições.

Imagine que o corpo de um loop precisa de ser executado exatamente cem vezes. Se desejar utilizar o loop while para o fazer, pode ser assim:
i = 0
while i < 100:
    # do_something()
    i += 1


Seria bom se alguém pudesse fazer esta contagem aborrecida por si. Isso é possível?

Claro que é - há um loop especial para estes tipos de tarefas, e é chamado for.

Na verdade, o loop for foi concebido para realizar tarefas mais complicadas - pode "navegar" por grandes coleções de dados item por item. Mostraremos como fazê-lo em breve, mas neste momento vamos apresentar uma variante mais simples da sua aplicação.

Dê uma vista de olhos no snippet:
for i in range(100):
    # do_something()
    pass


Existem alguns novos elementos. Deixe-nos falar sobre eles:

    a keyword for abre o loop for ; nota - não há nenhuma condição depois; não é preciso pensar nas condições, uma vez que são verificadas internamente, sem qualquer intervenção;
    qualquer variável após a keyword for é a variável de controlo do loop; conta as voltas do loop, e fá-lo automaticamente;
    a keyword in introduz um elemento de sintaxe que descreve a gama de valores possíveis que estão a ser atribuídos à variável de controlo;
    a função range() (esta é uma função muito especial) é responsável por gerar todos os valores desejados da variável de controlo; no nosso exemplo, a função irá criar (podemos mesmo dizer que irá alimentar o loop com) valores subsequentes a partir do conjunto seguinte: 0, 1, 2 .. 97, 98, 99; nota: neste caso, a função range() começa o seu trabalho a partir do 0 e termina um passo (um número inteiro) antes do valor do seu argumento;
    note a keyword pass dentro do corpo do loop - não faz nada; é uma instrução vazia - colocamo-la aqui porque a for sintaxe do laço exige pelo menos uma instrução dentro do corpo (a propósito - if, elif, else e while expressam a mesma coisa)

Os nossos próximos exemplos serão um pouco mais modestos no número de repetições do loop.


Veja o snippet abaixo. Consegue prever o seu output?
for i in range(10):
    print("The value of i is currently", i)


Execute o código para verificar se estava certo.

Nota:

    o loop foi executado dez vezes (é o argumento da função range() )
    o valor da última variável de controlo é 9 (não 10, visto começar a partir de 0, não a partir de 1)

A função range() pode ser equipada com dois argumentos, e não apenas um:
for i in range(2, 8):
    print("The value of i is currently", i)


Neste caso, o primeiro argumento determina o (primeiro) valor inicial da variável de controlo.

O último argumento mostra o primeiro valor que a variável de controlo não será atribuída.

Nota: a função range() aceita apenas inteiros como seus argumentos, e gera sequências de inteiros.

Consegue adivinhar o output do programa? Execute-o para verificar se também estava certo agora.

O primeiro valor mostrado é 2 (retirado do primeiro argumento range().)

O último é 7 (embora o range()segundo argumento seja 8).



for i in range(100):
    # do_something()
    pass

for i in range(2, 8):#argumentos son principio y final del rango
    print("The value of i is currently", i)
    
for i in range(2, 8, 3):
    print("The value of i is currently", i)
#The third argument is an increment - it's a value added to control the variable at every loop turn (as you may suspect, the default value of the increment is 1).

3.2.1.6 LAB: Essenciais do loop for - contar mississippily
Nível de dificuldade

Muito fácil
Objetivos

Familiarizar o aluno a:

    a utilização do loop for ;
    refletir situações da vida real em código informático.

Cenário

Sabe o que é o Mississippi? Bem, é o nome de um dos estados e rios dos Estados Unidos. O rio Mississippi tem cerca de 3.765 quilómetros de comprimento, o que o torna o segundo rio mais longo dos Estados Unidos (o mais longo sendo o rio Missouri). É tão longo que uma única gota de água precisa de 90 dias para percorrer toda a sua extensão!

A palavra Mississippi é também usada para um propósito ligeiramente diferente: contar mississippily.

Se não está familiarizado com a frase, estamos aqui para lhe explicar o seu significado: é usado para contar segundos.

A ideia por detrás disto é que adicionar a palavra Mississippi a um número ao contar segundos em voz alta faz com que soem mais perto do tempo do relógio, e por isso "um Mississippi, dois Mississippi, três Mississippi" levará aproximadamente três segundos de tempo real! É frequentemente utilizado por crianças que brincam às escondidas para garantir que o buscador faz uma contagem honesta.

A sua tarefa aqui é muito simples: escreva um programa que utilize um loop for para “contar mississippily” até cinco. Tendo contado até cinco, o programa deve imprimir para o ecrã a mensagem final "Ready or not, here I come!"

Use o esqueleto que fornecemos no editor.

INFORMAÇÃO EXTRA

Observe que o código no editor contém dois elementos que podem não estar totalmente claros para si neste momento: a declaração import time , e o método sleep() . Vamos falar sobre eles em breve.

Por enquanto, gostaríamos apenas que soubesse que importámos o módulo time e usámos o método sleep() para suspender a execução de cada função print() subsequente dentro do loop for por um segundo, para que a mensagem enviada para a consola se assemelhe a uma contagem real. Não se preocupe - em breve aprenderá mais sobre módulos e métodos.
Output esperado
1 Mississippi
2 Mississippi
3 Mississippi
4 Mississippi
5 Mississippi

LAB

import time

for i in range(5):
    print(i+1,"Mississippi" )# Body of the loop - print the loop iteration number and the word .
    time.sleep(1)# Body of the loop - use: time.sleep(1)

print("Ready or not, here I come!")# Write a print function with the final message.

END LAB

These two instructions are:

    break - exits the loop immediately, and unconditionally ends the loop's operation; the program begins to execute the nearest instruction after the loop's body;
    continue - behaves as if the program has suddenly reached the end of the body; the next turn is started and the condition expression is tested immediately.
CODE
# break - example

print("The break instruction:")
for i in range(1, 6):
    if i == 3:
        break
    print("Inside the loop.", i)
print("Outside the loop.")


# continue - example

print("\nThe continue instruction:")
for i in range(1, 6):
    if i == 3:
        continue
    print("Inside the loop.", i)
print("Outside the loop.")
END CODE

CODE
largestNumber = -99999999
counter = 0

while True:
    number = int(input("Enter a number or type -1 to end program: "))
    if number == -1:
        break
    counter += 1
    if number > largestNumber:
        largestNumber = number

if counter != 0:
    print("The largest number is", largestNumber)
else:
    print("You haven't entered any number.")
END CODE

Os loops break e declarações continue .

Até agora, temos tratado o corpo do loop como uma sequência indivisível e inseparável de instruções que são executadas completamente a cada volta do loop. No entanto, como programador, poderá ser confrontado com as seguintes escolhas:

    parece que é desnecessário continuar o loop como um todo; deve abster-se de continuar a execução do corpo do loop e continuar;
    parece que é necessário iniciar a próxima volta do loop sem completar a execução da volta atual.

O Python fornece duas instruções especiais para a execução de ambas estas tarefas. Digamos, por uma questão de precisão, que a sua existência na linguagem não é necessária - um programador experiente é capaz de codificar qualquer algoritmo sem estas instruções. Tais adições, que não melhoram o poder expressivo da linguagem, mas apenas simplificam o trabalho do programador, são por vezes chamadas de doces sintáticos, ou açúcar sintático.

Estas duas instruções são:

    break - sai imediatamente do loop, e termina incondicionalmente a operação do loop; o programa começa a executar a instrução mais próxima após o corpo do loop;
    continue - comporta-se como se o programa tivesse subitamente chegado ao fim do corpo; inicia-se a volta seguinte e a expressão da condição é testada imediatamente.

Ambas as palavras são keywords.

Agora vamos mostrar-lhe dois exemplos simples para ilustrar como as duas instruções funcionam. Veja o código no editor. Execute o programa e analise o output. Modifique o código e experimente.

CODE
largestNumber = -99999999
counter = 0

number = int(input("Enter a number or type -1 to end program: "))

while number != -1:
    if number == -1:
        continue
    counter += 1

    if number > largestNumber:
        largestNumber = number
    number = int(input("Enter a number or type -1 to end program: "))

if counter:
    print("The largest number is", largestNumber)
else:
    print("You haven't entered any number.")
END CODE

while True:
    # Write code in the body of the loop.
	# Put a conditional statement.
	    # Exit the loop here.
# Print the message.
The break statement is used to exit/terminate a loop.

Design a program that uses a while loop and continuously asks the user to enter a word unless the user enters "chupacabra" as the secret exit word, in which case the message "You've successfully left the loop." should be printed to the screen, and the loop should terminate.
_____________________
our program must:

    ask the user to enter a word;
    use userWord = userWord.upper() to convert the word entered by the user to upper case; we'll talk about the so-called string methods and the upper() method very soon - don't worry;
    use conditional execution and the continue statement to "eat" the following vowels A, E, I, O, U from the inputted word;
    print the uneaten letters to the screen, each one of them on a separate line.

Test your program with the data we've provided for you.


3.2.1.9 LAB: A declaração break - Preso num loop
Tempo estimado

10-20 minutos
Nível de dificuldade

Fácil
Objetivos

Familiarizar o aluno a:

    a utilização do loop break em loops;
    refletir situações da vida real em código informático.

Cenário

O comando break é utilizada para sair/terminar um loop.

Crie um programa que use um loop while e pede continuamente ao utilizador para introduzir uma palavra, a menos que o utilizador introduza "chupacabra" como a palavra secreta de saída, caso em que a mensagem "You've successfully left the loop." deve ser impressa para o ecrã, e o loop deve terminar.

Não imprima nenhuma das palavras introduzidas pelo utilizador. Utilize o conceito de execução condicional e a break declaração.


CODE
# Prompt the user to enter a word
userWord = input("Type a word: ")# and assign it to the userWord variable.
userWord = userWord.upper()
for letter in userWord:
    # Complete the body of the for loop.
    if letter == "A":
        continue
    if letter == "E":
        continue
    if letter == "I":
        continue
    if letter == "O":
        continue
    if letter == "U":
        continue
    print(letter)
    
 END CODE

Your program must:

    ask the user to enter a word;
    use userWord = userWord.upper() to convert the word entered by the user to upper case; we'll talk about the so-called string methods and the upper() method very soon - don't worry;
    use conditional execution and the continue statement to "eat" the following vowels A, E, I, O, U from the inputted word;
    assign the uneaten letters to the wordWithoutVovels variable and print the variable to the screen.

Look at the code in the editor. We've created wordWithoutVovels and assigned an empty string to it. Use concatenation operation to ask Python to combine selected letters into a longer string during subsequent loop turns, and assign it to the wordWithoutVovels variable.

     3.2.1.10 LAB: A declaração continue - o Ugly Vowel Eater

Tempo estimado

10-20 minutos
Nível de dificuldade

Fácil
Objetivos

Familiarizar o aluno a:

    a utilização do loop continue em loops;
    refletir situações da vida real em código informático.

Cenário

O comando continue é utilizada para saltar o bloco atual e avançar para a próxima iteração, sem executar as declarações dentro do loop.

Pode ser utilizada tanto com os loops while e for .

A sua tarefa aqui é muito especial: tem de conceber um vowel eater (comedor de vogais)! Escreva um programa que use:

    um loop for ;
    o conceito de execução condicional (if-elif-else)
    a declaração continue .

O seu programa deve:

    pedir ao utilizador para introduzir uma palavra;
    usar user_word = user_word.upper() para converter a palavra introduzida pelo utilizador em maiúsculas; falaremos sobre os chamados métodos de strings e o método upper() muito em breve - não se preocupe;
    usar execução condicional e a declaração continue para “comer” as seguintes vogais A, E, I, O, U da palavra introduzida;
    imprimir as letras não comidas para o ecrã, cada uma delas numa linha separada.

Teste o seu programa com os dados que lhe fornecemos.

Dados de teste

Input de amostra: Gregory

Output esperado:
G
R
G
R
Y

Input de amostra: abstemious

Output esperado:
B
S
T
M
S

Input de amostra: IOUEA

Output esperado: 

https://edube.org/sandbox/058cc7fc-50ca-11ec-9e68-0242157e55ca

 3.2.1.11 LAB: A declaração continue - o Pretty Vowel Eater
Tempo estimado

5-15 minutos
Nível de dificuldade

Fácil
Objetivos

Familiarizar o aluno a:

    a utilização do loop continue em loops;
    modificar e atualizar o código existente;
    refletir situações da vida real em código informático.

Cenário

A sua tarefa aqui é ainda mais especial do que antes: deve redesenhar o comedor de vogais (feio) do laboratório anterior (3.1.2.10) e criar um comedor de vogais (bonito) melhor e mais aperfeiçoado! Escreva um programa que use:

    um loop for ;
    o conceito de execução condicional (if-elif-else)
    a declaração continue .

O seu programa deve:

    pedir ao utilizador para introduzir uma palavra;
    usar user_word = user_word.upper() para converter a palavra introduzida pelo utilizador em maiúsculas; falaremos sobre os chamados métodos de strings e o método upper() muito em breve - não se preocupe;
    usar execução condicional e a declaração continue para “comer” as seguintes vogais A, E, I, O, U da palavra introduzida;
    atribuir as letras não comidas à variável word_without_vowels e imprimir a variável para o ecrã.

Veja o código no editor. Criámos word_without_vowels e atribuimos-lhe uma string vazia. Utilize a operação de concatenação para pedir ao Python que combine as letras selecionadas numa string mais longa durante os loops subsequentes, e atribua-a à variável word_without_vowels .

Teste o seu programa com os dados que lhe fornecemos.

Dados de teste

Input de amostra: Gregory

Output esperado:
GRGRY

Input de amostra: abstemious

Output esperado:
BSTMS

CODE
wordWithoutVovels = ""

# Prompt the user to enter a word
userWord = input("Type a word: ")# and assign it to the userWord variable
userWord = userWord.upper()

for letter in userWord:
    if letter == "A":
        continue
    if letter == "E":
        continue
    if letter == "I":
        continue
    if letter == "O":
        continue
    if letter == "U":
        continue
    wordWithoutVovels = wordWithoutVovels + letter
print(wordWithoutVovels)
END CODE
WHILE AND FOR HAVE AN ELSE  SENTENCE WHICH SHOWS THE FALSE FINAL RESULT

  
