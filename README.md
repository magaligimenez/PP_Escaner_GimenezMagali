# Escaner libros y mapas
Biblioteca de clases desarrollada por Gimenez Magali. Para ver el enunciado hacer click aquí: [Enunciado](https://www.utnfravirtual.org.ar/pluginfile.php/545997/mod_resource/content/1/PP_Escaner.pdf)

## Sobre mí:
Mi nombre es Magali Gimenez, estudiante de la UTN. para mi fue un gran desafio realizar este trabajo pero muy divertido. Me sorprendió mucho para bien e intenté aplicar todo lo visto en clase para poder desarrollar el codigo de la mejor forma posible. 

## Resumen:
El ejercicio consta de dos documentos, Mapas y libros. Cada uno de ellos debe poder escanearse, pero con algunas condiciones:
- No debe escanear los mismos libros y mapas.
- No se debe poder agregar un mapa al escaner del libro y viceversa.
- No contienen las mismas propiedades (es decir, atributos)
- Pueden encontrarse en los estados:
  - inicio
  - distribuido
  - enEscaner
  - enRevision
  - terminado
- Se debe verificar antes de avanzar a otro estado, que no se encuentren en el último (terminado).

## Diagrama de clases:

![Captura de pantalla 2024-05-22 033155](https://github.com/magaligimenez/PP_Escaner_GimenezMagali/assets/123522629/92b5ae97-f007-4c55-8d9c-1a31fbe41082)

## Justificacion Tecnica:

* Introduccion a .NET y C#
* Clases y metodos estáticos
  * Clase estática Informes: Al ser una clase que contiene la informacion de la lista y hardcodea los datos. No necesito instanciarlos.
 
* Abstraccion:
  * Mediante la abstracción pude identificar que era importante y que no incluir dentro de cada una de las clases.

* Encapsulamiento:
  * Gracias a este pilar logré definir que atributos debian ser visibles en todo el programa y cuales no. Usé las propiedades GET en la mayoría y fueron de gran utilidad.
 
* Herencia:
  * Logré no repetir código utilizando la herencia, realicé la clase padre llamada Documento de la cual la heredaban Libro y Mapa.
 
* Polimorfismo:
  * Lo apliqué esencialmente en el método ToString(). Fue de gran ayuda para optimizar el código.

* Sobrecargas de operadores:
  * Me fueron de gran ayuda para poder definir igualdades tanto en Libro, Mapa y Escaner. Ademas utilicé la sobrecarga del operador + para la clase Escaner así verificaba si podía agregar el libro o mapa deseado a la lista correspondiente
 
* Colecciones: Uso de listas para almacenar mapas o libros.
