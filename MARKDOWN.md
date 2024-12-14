# Markdown
**Markdown** es un lenguaje de marcado ligero creado por [John Gruber](https://es.wikipedia.org/w/index.php?title=John_Gruber&action=edit&redlink=1 "John Gruber (aún no redactado)") y [Aaron Swartz](https://es.wikipedia.org/wiki/Aaron_Swartz "Aaron Swartz") que trata de conseguir la máxima legibilidad y facilidad de publicación tanto en su forma de entrada como de salida, inspirándose en muchas convenciones existentes para marcar mensajes de correo electrónico usando texto plano.
[Más información](https://es.wikipedia.org/wiki/Markdown)
## Sintaxis
### Encabezados
Establecen los títulos de las secciones del documento Markdown a distintos niveles. Son el equivalente a los `h1`-`h6` de HTML.
```markdown
# Encabezado de nivel 1
## Encabezado de nivel 2
### Encabezado de nivel 3
#### Encabezado de nivel 4
##### Encabezado de nivel 5
###### Encabezado de nivel 6
```
### Cursiva
El texto que se quiera mostrar en *cursiva* debe estar encerrado entre dos asteriscos (`*`).
`La palabra *cursiva* está encerrada entre asteriscos.`
### Negrita
El texto en **negrita** se obtiene encerrando el texto entre asteriscos dobles `**`.
`El texto **en negrita** está encerrado entre asteriscos dobles.`
### Índices
Los índices son caracteres más pequeños de lo normal utilizados en ciertas notaciones. Existen dos tipos: __superíndice__ y __subíndice__.
#### Superíndice 
Está desplazado hacia arriba. Se suele utilizar, por ejemplo, para marcar el exponente de una potencia. Por ejemplo, x^2^. Se marca encerrando el texto entre dos tejados (`^`),
```markdown
3^2^ = 9
```
### Saltos de línea y párrafos
La diferencia entre el salto de línea y un párrafo es un `Enter`. Es decir, para hacer un **salto de línea**, pulsaremos `Enter` una vez (lo que equivales a `<br>` en HTML). Para hacer un nuevo párrafo, pulsaremos dos veces `Enter` (lo que equivales a `<p></p>` en HTML).
```markdown
Esto es una línea.
Esto es otra línea, separada de la anterior por un salto de línea.

Esto es un párrafo.

Esto es otro párrafo.
```
### Listas
Las listas son una agrupación de tareas o instrucciones que guardan una relación en común. Con Markdown podemos definir tres tipos de listas: desordenadas, ordenadas y de tareas.
##### Listas desordenadas
Los elementos de este tipo de listas no tienen un orden específico. Equivalen a `<ul>` de HTML. Los elementos de esta lista se definen empezando con un guión (`-`) o un asterisco (`*`) y un espacio (`-`). Si necestiamos hacer subniveles de la lista, tendremos que añadir tabulaciones delante.
```markdown
## Oferta de trabajo
- __Requisitos requeridos__
	- Titulación técnica
	- Nivel B2 o superior de inglés
	- 2 años de experiencia en la posición
* __Requisitos deseados__
	* Nivel B1 o superior de alemán
	* 1 años de experiencia como jefe de proyecto
	* Master en dirección de empresas
```
##### Listas ordenadas
Al contrario que las anteriores, este tipo de listas están pensadas para seguirlas en orden, del primer elemento a último. Suelen usarse para describir procesos. Su sintaxis es usar un número seguido de un punto (`.`) y un espacio.
```markdown
## Huevo cocido
1. Coger olla o cazuela
2. Llenar de agua
3. Poner a calentar hasta que hierva
4. Introducir el huevo crudo en el agua
5. Esperar 12 minutos
6. Sacar huevo
```
##### Listas de tareas
En este tipo de listas se definen tareas a realizar. Cada elemento de esta listas tiene un check para indicar su estado, que puede ser:
- **Pendiente**: Indica que la tarea aún no se ha realizado. El check está vacío. El texto de ir precedido de `- [ ]` .
- **Realizado**: Indica que la tarea se ha completado. El check está marcado. El texto de ir precedido de `- [x]` .
Como de puede apreciar, la única diferencia entre el prefijo de un elemento pendiente y uno realizado es que en el primero dentro de los corchetes hay un espacio y en el segundo hay una `x`.
```markdown
## Compra supermercado
- [x] 1 kg de aguacates
- [ ] 1 kg de tomates
- [x] 2 litros de leche desnatada
- [ ] Pack yogures desnatados fresa
```
### Texto monoespaciado
El texto monoespaciado es aquél que todos los caracteres ocupanel mismo espacio. Normalmente es usado para representar texto de algún lenguaje de programación. Se utiliza encerrando el texto entr dos acentos graves (`` ` ``).
Para insertar una imagen en HTML usamos la etiqueta `<img>`.
### Código
Si necesitamos insertar fragmentos de código en nuestro documento Markdown, debemos generar un bloque que empiece y termine con tres acentos graves. Si los tres primeros acentos los seguimos de un [identificador de lenguaje](https://github.com/jincheng9/markdown_supported_languages), el texto se coloreará siguiendo la sintaxis.
![Ejemplo de bloque de código SQL](/assets/markdown/markdown_code.png)


### Tablas
Las tablas definen sus columnas con una tubería (`|`). 
Los encabezados están separados por el resto de filas por celdas rellenas con guiones (`-`). Solo es necesario un guión, aunque se pueden añadir todos los que se deseen, para que quede mejor formateado el texto.
```markdown
| Ciudad | País | Continente |
|-|-|-|
|Madrid|España|Europa|
|Toronto|Canadá|América|
|Sydney|Australia|Oceanía|
|Rabat|Marruecos|África|
```
En la fila de separación de las cabeceras (`|-|`) se puede definir la alineación de las columnas, incluída la cabecera.
- `:-` Alinea la columna a la izquierda
- `:-:` Alinea la columna al centro
- `-:` Alinea la columna a la derecha

| Tarea | Progreso | Finalizada |
|:-|-:|:-:|
|Toma de requisitos|100%|SÍ|
|Desarrollo del módulo principal|68%|NO|
|Documentación|0%|NO|
