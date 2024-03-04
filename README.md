#Dada una cadena larga de 5 párrafos elabora las estadísticas correspondientes en la cual se controlen los datos mediante las siguientes listas:
letras = ['abcdefghijklmnñopqrstuvwxyz']
caracteres =['a','e','i', 'o','u', ' ', ',','.' ]
estadisticas = ['Total de caracteres:', 'Total de letras : ', 'Total de vocales a :', 'Total de vocales e :', 'Total de vocales i :', 'Total de vocales o :', 'Total de vocales u :', 'Total de espacios :', 'Total de comas', 'Total de puntos']
totales = [1,1,0,0,0,1,0,0,0,0]

#
#Ejemplo de salida:
cadenaLarga = """
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc placerat egestas egestas. Morbi malesuada eros sed odio mattis luctus ut quis libero. Nunc tincidunt sapien at congue sodales. Praesent a maximus libero. Proin sed placerat elit, condimentum vulputate nunc. Quisque et sodales nisi. Nulla elementum ex in odio ultrices malesuada. Praesent dictum ante sit amet enim semper scelerisque. Pellentesque eros massa, dapibus at mi eget, ullamcorper aliquet leo. Nulla id lacus id dui convallis dapibus. Aliquam vitae mattis leo. Vivamus elementum, metus elementum eleifend vehicula, magna enim consequat ante, imperdiet blandit elit diam sed urna. Vivamus finibus maximus elit ut laoreet. Aliquam fringilla rhoncus dapibus. Donec in consequat lorem. Sed vestibulum facilisis egestas.

Proin in convallis augue. Vestibulum elementum nibh et urna pellentesque, quis blandit tortor tempor. Vivamus tristique condimentum rutrum. Aliquam at odio facilisis, convallis lorem sit amet, posuere odio. Integer aliquet in felis tristique scelerisque. Duis finibus at velit in eleifend. Integer sed ligula consectetur, sollicitudin nisl at, tempor purus. Curabitur consequat ante nec lorem interdum feugiat. Etiam sagittis ornare ex, vitae tempus purus commodo eget. Curabitur tempor dui nunc, at ultrices ligula condimentum eget. Mauris ac ante viverra, sodales arcu eget, mattis mi. Pellentesque condimentum hendrerit sem. Sed tincidunt bibendum augue a dapibus. Nam quis eleifend magna.
"""
print(cadenaLarga)
letras = ['abcdefghijklmnñopqrstuvwxyz']
caracteres =['a','e','i', 'o','u', ' ', ',','.' ]
estadisticas = ['Total de caracteres:', 'Total de letras : ', 'Total de vocales a :', 'Total de vocales e :', 'Total de vocales i :', 'Total de vocales o :', 'Total de vocales u :', 'Total de espacios :', 'Total de comas', 'Total de puntos']
totales = [1,1,0,0,0,1,0,0,0,0]

#Presentar un resumen de las estadística de los párrafos
#otal de caracteres:
#Total de letras :
#Total de vocales a :
#Total de vocales e :
#Total de vocales i :
#Total de vocales o :
#Total de vocales u :
#Total de espacios :
#Total de comas :
#total de puntos :

#Algoritmo
#1. Crear lista cadenaLarga
#2. Crear lista caracteres
#3. Crear lista de estadisticas
#4. Crear lista totales
#5. Recorrer cadenaLarga
#6.      Ir acumulando los valores de totales según caracteres
#7. Imprimir totales tomando los valores de las listas 'estadisticas' y 'totales'

cadenaLarga = """
Tu cadena larga de 5 párrafos aquí...
"""

letras = 'abcdefghijklmnñopqrstuvwxyz'
caracteres =['a','e','i', 'o','u', ' ', ',','.' ]
estadisticas = ['Total de caracteres:', 'Total de letras : ', 'Total de vocales a :', 'Total de vocales e :', 'Total de vocales i :', 'Total de vocales o :', 'Total de vocales u :', 'Total de espacios :', 'Total de comas:', 'Total de puntos:']
totales = [0] * len(estadisticas)

for char in cadenaLarga:
    totales[0] += 1  # Total de caracteres
    if char in letras:
        totales[1] += 1  # Total de letras
    if char in caracteres[0]:
        totales[2] += 1  # Total de vocales a
    elif char in caracteres[1]:
        totales[3] += 1  # Total de vocales e
    elif char in caracteres[2]:
        totales[4] += 1  # Total de vocales i
    elif char in caracteres[3]:
        totales[5] += 1  # Total de vocales o
    elif char in caracteres[4]:
        totales[6] += 1  # Total de vocales u
    elif char == ' ':
        totales[7] += 1  # Total de espacios
    elif char == ',':
        totales[8] += 1  # Total de comas
    elif char == '.':
        totales[9] += 1  # Total de puntos

print("Resumen de estadísticas:")
for i in range(len(estadisticas)):
    print(estadisticas[i], totales[i])

