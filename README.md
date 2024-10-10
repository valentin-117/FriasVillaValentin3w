# FriasVillaValentin3w
#saludo
              
              print("")


           print("Este es un programa que imprimirá  un saludo cada vez que sea requerido. ")#imprime la funcion del programa 

           print("")

         print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
         

          print("")

     def imprimir_saludo(): #def para definir el saludo

    #imprime el saludo en la consola
    
            print("¡¡HEY AMIGOS!!")

      # La funcion "if" es la función principal aqui


      if __name__ == "__main__":

    # Bucle infinito que permite al usuario interactuar con el programa
    while True:
    
           #solicita al usuario ingresar el mensaje
           
                                entrada = input("Escribe ´hola´ para ver el mensaje o ´salir´ para terminar: ")
                                
        #verifica si el usuario escribió "hola"
        if entrada.lower() == 'hola':
            imprimir_saludo()  # Llama a la función para imprimir 'hola'
        
        elif entrada.lower() == 'salir':#verifica si el usuario escribió "salir"
            print("Saliendo del programa.")  
            break  #termina el bucle
        else:
            print("Comando no reconocido.") #imprime este mensaje si el comando  ingresado por el usuario es incorrecto


![image](https://github.com/user-attachments/assets/5321313e-d3b0-4ddf-8bcb-0ea7d8501e13)

#saludo 2

    print("")
    print("Este es un programa que imprimirá tu nombre y un saludo despues de pedirtelo. ")#imprime la funcion del programa 
    print("")
      print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
     print("")
    #pide al usuario ingresar su nombre
    nombre= input("Ingresa tu nombre: ")
    #imprime el saludo
     print("HOLAA ",nombre)
![image](https://github.com/user-attachments/assets/152e7eee-c69a-4043-ab14-3283fabfd4d5)

#IVA

     print("")
     print("Este es un programa que calculará el IVA. ")#imprime la funcion del programa 
    print("")
    print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
    print("")
    def calcular_total_con_iva(cantidad_sin_iva, porcentaje_iva):

    iva = (cantidad_sin_iva * porcentaje_iva) / 100  #calcula el IVA
    total = cantidad_sin_iva + iva  # Suma el IVA al monto original
     return total  # Devuelve el total
    # Solicitar al usuario la cantidad sin IVA
    cantidad_sin_iva = input("Introduce la cantidad sin IVA: ")
     #solicitar el porcentaje de IVA
       porcentaje_iva = input("Introduce el porcentaje de IVA a aplicar: ")
        try:
    #Convertimos las entradas a float
    cantidad_sin_iva = float(cantidad_sin_iva)  
    porcentaje_iva = float(porcentaje_iva) 
    #se asegura de que los valores sean no negativo
    if cantidad_sin_iva < 0 or porcentaje_iva < 0:
        print("La cantidad y el porcentaje deben ser números no negativos.")
    else:
        total_con_iva = calcular_total_con_iva(cantidad_sin_iva, porcentaje_iva)
        print(f"El total de la factura, incluyendo el IVA, es: {total_con_iva:.2f}")#imprime el resultado en pantalla
      except ValueError:
    print("Entrada inválida. Asegúrate de introducir números válidos.")#Manejo de errores si el parametro no es válido
  ![image](https://github.com/user-attachments/assets/33630515-8ef8-40ce-801c-5906d90bea40)

  #FRASE
  
    print("")
    print("Este es un programa que nos dirá el tamaño en numeros enteros de lla ultima palabra d una frase. ")#imprime la funcion del programa 
     print("")
      print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
     print("")
    def tam_ultima_palabra(frase):

    #se separa la frase en palabras usando split(), que maneja múltiples espacios
    palabras = frase.split()
    if palabras:  # Verificamos si hay palabras en la lista
        return len(palabras[-1])  #devolvemos la longitud de la última palabra
    return 0  #se devuelve si no hay palabras

     #solicitar al usuario una frase
    frase = input("Introduce una frase: ")

     #imprime el resultado
    Longitud = tam_ultima_palabra(frase)
     print(f"La longitud de la última palabra es: {longitud}")
  ![image](https://github.com/user-attachments/assets/ef25d895-5551-4aee-8571-fbff5c6dfd21)
#MAYOR

     print("")
    print("Este es un programa que nos dirá cual es el mayor de los numeros que ingresemos ")#imprime la funcion del programa 
    print("")
    print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
     print("")
    numero1 = int(input("Introduce el primer número: "))
    numero2 = int(input("Introduce el segundo número: "))
     numero3 = int(input("Introduce el tercer número: "))

     # Calcular el mayor y mostrar el resultado
     mayor =max(numero1, numero2, numero3)
     print(f"El mayor de los tres números es: {mayor}") 
![image](https://github.com/user-attachments/assets/1a214add-3fd6-4782-83f0-ee76b8f03ac5)

#FACTORIAL

     print("")
     print("Este es un programa que te dará el factorial del numero que le asignes. ")#imprime la funcion del programa 
     print("")
      print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
     print("")
     def calcular_factorial(n):
    resultado = 1 
    if n == 0 or n == 1:
        return resultado #indica que el factorial de 0 es 1
    else:
        for i in range(2, n + 1):
            resultado *= i #se realiza la operación
    return resultado  # Devolvemos el resultado final

        #pide al usuario ingresar el numero deseado
     numero = input("Introduce un entero positivo: ")
        try:
    numero = int(numero) #se declara la entrada de numeros como enteros
    if numero < 0:
        print("Debes introducir un número entero positivo.")#recuerda al usuario en caso de haber introducido un numero negativo
    else:
        print(f"El factorial de {numero} es {calcular_factorial(numero)}.")#imprime en pantalla el resultado
    except ValueError:
    print("Entrada inválida. Introduce un número entero.")#indica que el numero ingresado no es valido

![image](https://github.com/user-attachments/assets/ff8bfbc2-1713-4e5f-a75b-a990544ca044)

#AREAS

     print("")
     #imprime la funcion del programa 
     print("Este es un programa que realizara las operaciones para sacar el area de un circulo y el volumen de un. ")
     print("")
     print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
    print("")
    import math
    def calcular_area_circulo(radio):
    area = math.pi * (radio ** 2)  #realiza la operación para sacar el radio del circulo
    return area  #devuelve el area capturada

    def calcular_volumen_cil(radio, altura):
    area_base = calcular_area_circulo(radio)  #calcula el area del circulo
    volumen = area_base * altura  #realiza la formula de el volumen
    return volumen #devuelve el volumen 
     #solicita al usuario ingresar los datos
     radio = input("Introduce el radio del círculo: ")
     altura = input("Introduce la altura del cilindro: ")
    try:
    #las entradas se convierten a numeros reales
    radio = float(radio)
    altura = float(altura)

    #revisa que los numeros no sean negativos
    if radio < 0 or altura < 0:
        print("El radio y la altura deben ser números no negativos.")
    else:
        #calcula el área del círculo
        area_circulo = calcular_area_circulo(radio)
        print(f"El área del círculo es: {area_circulo:.2f}")
        #calcula el volumen del cilindro
        volumen_cilindro = calcular_volumen_cil(radio, altura)
        print(f"El volumen del cilindro es: {volumen_cilindro:.2f}")
        
     except ValueError:
    #revisa si los datos obtenidos son validos
    print("Entrada inválida. Asegúrate de introducir números válidos.")

![image](https://github.com/user-attachments/assets/8d229119-05d8-41fd-baf1-692a74c0ee1b)

#GMAIL

     print("")
     print("Este es un programa que nos dirá si una dirección de correo es valida. ")#imprime la funcion del programa 
      print("")
     print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
     print("")
    def es_email_valido(email):
    return '@' in email #verifica que el correo contenga el carácter '@'
    def main():
    # Solicita al usuario que introduzca su dirección de email
    email = input("Introduce tu dirección de email: ")
    
    #verificacion
    if es_email_valido(email):
        print(f"La dirección de email es válida: {email}") #imprime que el correo es valido
    else:
        print("La dirección de email no es válida.") #imprime que el correo no es valido debido a que falta un carácter
      if __name__ == "__main__":
    main()
![image](https://github.com/user-attachments/assets/8fd46f1a-6b11-4726-a583-932f841066ac)

#SUMA_MULT

    print("")
    print("Este es un programa que nos dirá la suma y multiplicacion de los numeros 1, 2, 3 y 4 ")#imprime la funcion del programa 
     print("")
     print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
     print("")
    def sum(lista):

    total = 0  # Inicializa el total en 0
    for numero in lista:  #Itera sobre cada número en la lista
        total += numero  #suma cada número al total
    return total  

    def multip(lista):
    producto = 1  #inicializa el producto en 1
    for numero in lista:  #itera sobre cada número en la lista
        producto *= numero  #multiplica cada número al producto
    return producto  #devuelve el producto acumulado

    def main():
    #lista de números para probar las funciones
    numeros = [1, 2, 3, 4]
    #calcula la suma de la lista de números
    resultado_suma = sum(numeros)
    #calcula la multiplicación de la lista de números
    resultado_multiplicacion = multip(numeros)
    
    #muestra los resultados de la suma y multiplicación
    print(f"La suma de {numeros} es: {resultado_suma}")
    print(f"La multiplicación de {numeros} es: {resultado_multiplicacion}")
     if __name__ == "__main__":

    main()  
![image](https://github.com/user-attachments/assets/dd22b623-8e44-42b6-82ea-a4972e405362)

#VOCAL

     print("")
     print("Este es un programa que nos dira si el carácter ingresado es una vocal o no. ")#imprime la funcion del programa 
     print("")
    print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
     print("")
     def es_vocal(caracter):
    #definimos las vocales en mayúsculas y minúsculas
    vocales = 'aeiouAEIOU'
    
    #verificamos si el carácter está en la cadena de vocales
    return caracter in vocales
     def main():
    # Solicita al usuario que introduzca un carácter
    caracter = input("Introduce un carácter: ")
    
    # Verifica que el usuario introduzca solo un carácter
    if len(caracter) != 1:
        print("Por favor, introduce solo un carácter.") #se pide al usuario ingresar un solo caracter
        return  
    #verificacion de si es vocal o no
    if es_vocal(caracter):
        print(f"El carácter '{caracter}' es una vocal.")  #imprime un mensaje de que si es una vocal
    else:
        print(f"El carácter '{caracter}' no es una vocal.") #imprime un mensaje de que no es una vocal
     #funcion principal
     if __name__ == "__main__":
    main()  

![image](https://github.com/user-attachments/assets/fdda4533-0846-4193-a60b-4f97a745e06a)

#COORDENADAS

      print("")
     print("Este es un programa que dará la distancia de un punto y otro. ")#imprime la funcion del programa 
      print("")
      print("Frías Villa Angel Valentin 3W. ") #imprime mi nombre
     print("")

     import math
     def calcular_distancia(punto1, punto2):
    #coordenadas de los puntos
    x1, y1 = punto1
    x2, y2 = punto2
    #se aplica la formula de la disstancia
    distancia = math.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
    return distancia

    def main():
    # Solicita al usuario las coordenadas del primer punto
    x1 = float(input("Introduce la coordenada x del primer punto: "))
    y1 = float(input("Introduce la coordenada y del primer punto: "))
    
    #se pide al usuario las coordenadas del segundo punto
    x2 = float(input("Introduce la coordenada x del segundo punto: "))
    y2 = float(input("Introduce la coordenada y del segundo punto: "))
    #se calcula la distancia
    distancia = calcular_distancia((x1, y1), (x2, y2))
    #muestra el resultado
    print(f"La distancia entre los puntos ({x1}, {y1}) y ({x2}, {y2}) es: {distancia:.2f}")

     if __name__ == "__main__":
    # funcion principal
    main()

![image](https://github.com/user-attachments/assets/9bdcb52f-5c1a-4422-bc02-9cbe88dcc4cb)



