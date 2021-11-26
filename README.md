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

The comment are made with the # symbol
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

input() function supports arguments and captures strings
input("Esta pregunta aparece sin problema: ")

Type casting
Las funciones int() y float() sirven para cambiar el tipo de dato ingresado

e.g. 
anything = float(input("Enter a number: "))
something = anything ** 2.0
print(anything, "to the power of 2 is", something)

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

for i in range(100):
    # do_something()
    pass

for i in range(2, 8):#argumentos son principio y final del rango
    print("The value of i is currently", i)
    
for i in range(2, 8, 3):
    print("The value of i is currently", i)
#The third argument is an increment - it's a value added to control the variable at every loop turn (as you may suspect, the default value of the increment is 1).

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

3.1.2.14 LAB
  
