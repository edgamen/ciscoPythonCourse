# ciscoPythonCourse
Notas curso Python de Cisco

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
    
 

