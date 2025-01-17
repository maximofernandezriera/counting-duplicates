# Counting duplicates kata

### Debemos implementar una función que cuente el número de caracteres alfabéticos en mayúsculas y minúsculas y dígitos numéricos distintos que aparecen más de una vez en una cadena de entrada.

#### Podemos suponer que la cadena de entrada contiene solo alfabetos (tanto mayúsculas como minúsculas) y dígitos numéricos.

* https://www.codewars.com/kata/54bf1c2cd5b56cc47f0007a1

_________________________________________________________________________________________________________
_________________________________________________________________________________________________________
_________________________________________________________________________________________________________
_________________________________________________________________________________________________________

## PSEUDOCÓDIGO

      // Convertir el texto a minúsculas para que 'a' y 'A' se consideren iguales
      texto = texto.aMayusculas()
    
      // Crear una estructura de datos para almacenar los caracteres que ya hemos contado
      caracteresContados = Estructura() 
    
      // Crear un contador para almacenar el número de duplicados
      contadorDuplicados = 0 
    
      // Recorrer cada carácter del texto
      Para cada caracter en texto
        // Si el carácter ya está en el conjunto 'caracteresContados', significa que es un duplicado
        Si caracter está en caracteresContados:
          // Incrementa el contador de duplicados
          contadorDuplicados = contadorDuplicados + 1 
        // Si no, añade el carácter al conjunto para que no lo contemos de nuevo
        Sino
          caracteresContados.añadir(caracter)
    
      // Devolver el número total de duplicados encontrados
      Devolver contadorDuplicados 

