# Sintaxis

### **Espacios**
Los espacios y sangrías al inicio y al final de un renglón son omitidos. Únicamente se visualizan los espacios entre caracteres. Más de un espacio se interpreta como uno solo.

### **Salto de línea**
Un único cambio de línea (\n) se interpreta como un cambio de línea. 

```
Primera línea
Segunda línea
```

### **Párrafos**
Más de un cambio de línea que es igual a más de un renglón vacío se interpreta como el fin de un párrafo y el inicio de otro. Más de un renglón vacío se interpreta como solo uno.

```
Primer párrafo

Segundo párrafo
```

### **Títulos y subtítulos**
Los títulos y subtítulos se identifican con uno o más símbolos numerales (#) con un espacio entre estos y el texto titular. A mayor símbolos numerales, mayor el nivel titular. 

```
# H1
## H2
### H3
...
```

### **Itálica** 
Estilo de fuente identificada con un par de asteriscos. No se dejan espacios entre los asteriscos y el texto. 

```
*Itálica*
```

### **Negrita**
Tipo de letra identificada con dos pares de asteriscos. No se dejan espacios entre los asteriscos y el texto.

```
**Negrita**
```

### **Itálica y negrita**
Tipo de letra identificada con tres pares de asteriscos. No se dejan espacios entre los asteriscos y el texto.
```
***Itálica y negrita***
```

### **Tachado**
Tipo de letra identificada con dos pares de virgulillas. No se dejan espacios entre los virgulilla y el texto.
```
~~Texto tachado~~
```

### **Bloque de cita**
Las citas se colocan en bloques marcados por un símbolos mayor que (>). Es necesario dejar un espacio entre el símbolo y el texto. 
```
> Bloque de cita
```
```
> Primer párrafo de cita
>
> Segundo párrafo de cita
```


### **Listas**
Las listas no ordenadas se identifican con dos guiones (--) seguidos de un espacio.
```
-- Elemento
-- Elemento
-- Elemento
```


### **Notas al pie de página**
Los pies de página o notas están en dos partes del documento. Primero en el texto donde se necesita hacer la aclaración o extensión. Luego al final del documento donde se establece la nota. Se hace uso de los símbolos mayor y menor (<>) para delimitar el texto a explicar. 

```
Texto donde se hace referencia a la <nota[^1]>.
```

```
[^1]: La nota.
```

### **Link**

Hay varias formas de crear un link. Primero aquella donde se desea visualizar el link tal y como es: 

```
[](https://www.example.com)
```

Segundo donde se desea visualizar la descripción del link en lugar del link mismo: 

```
[Descripción](https://www.example.com)
```

Y en el tercero se desea abrir el link en la misma ventana actual, generalemente para links dentro de la misma página:

```
[Descripción](https://www.example.com){sametab}
```

### Imagen

Se presentan 3 tipos de imágenes. 
La primera de ellas es aquella que no presenta un pie de imagen. Esta debe de tener un título para el tag alt en HTML, el link donde está la imagen y el ancho de la imagen con su unidad respectiva. 

```
![Título](link.jpg)(100%)
```

El segundo tipo de imagen es similar a la anterior pero incluye un pie de imagen, el cual se coloca entre asteriscos en la línea siguiente:

```
![Título](link.jpg)(100%)
*Pie de imagen*
```

El último tipo de imagen es aquella que al mismo tiempo es un link externo, generalmente para los iconos de redes sociales ligadas. La sintaxis es: 

![Título](link.jpg)(45px)(link externo)


### Audio

Los audios deben tener un título para el tag alt en HTML y el link donde se encuentra. 

```
!![Título](link.mp3)
```

### Código
Para escribir texto que no se debe interpretar por este lenguage, el texto debe ser colocado entre dos pares de 3 acentos graves (```):


```
&#96;&#96;&#96	
**Texto que no está en negrita**
&#96;&#96;&#96	
```

### Metadatos

Los metadatos se colocan el inicio del documento. Cada metadato se coloca después de dos barras (//) y un espacio.

```
&#47;&#47; LANGUAGE: es
&#47;&#47; AUTHOR: Laylah Rain
&#47;&#47; YEAR: 2020
```

### Texto principal

El texto principal del documento (como las trascripciones, ediciones y normas) se colocan entre los siguientes dos separadores: 

```
&#45;&#45;&#45;&#45;START_TEXT&#45;&#45;&#45;&#45;

Texto principal

&#45;&#45;&#45;&#45;END_TEXT&#45;&#45;&#45;&#45;
```

### Detalles 

Los detalles no forman parte del texto principal, estas secciones se usan para dar información complementaria: licencias, recomendaciones de lectura, referencias ... 
Cada sección de detalle debe tener un título, el cual se coloca después del símbolo numeral (#).


```
/&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;
# Titulo de la sección 

Texto de la sección

&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;/
```

### Pie de html

Al final de un documento html se coloca el pie de este. El pie se escribe igual que una sección de detalles pero sin el titular. 

```
/&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45; 

Texto del pie de html

&#45;&#45;&#45;&#45;&#45;&#45;&#45;&#45;/
```

Por arreglar:

Las listas ordenadas se identifican por los números seguidos de un punto y un espacio.
```
1. Primer elemento
2. Segundo elemento
3. Tercer elemento
```

Por último está la imagen a usar unicamente en la creación de pdfs para cubrir una página completa. La imagen debe de estar en formato PDF y debe tener el tamaño del documento final.  

```
![link.pdf]
```

## Algunas sintaxis extra aún en desarrollo para exportar a .tex

### Sangría
Una sangría se crea por medio del símbolo + al inicio del renglón. Se usa unicamente para dar estilo en la creación de PDF's.

```
+ Párrafo
```

### Renglón vacío
Un renglon vacío se crea por medio de los símbolos ++ en un renglón. Los símbolos deben de estar seguidos y se usa únicamente para dar estilo en la creación de PDF's.

```
++
```

### Cambio de página
Un cambio de página se crea por medio de los símbolos +++  en un renglón vacío. Los símbolos deben de estar seguidos y se usa únicamente para dar estilo en la creación de PDF's.

```
+++
```

### Imagen 

Imagen a usar unicamente en la creación de pdfs para cubrir una página completa. La imagen debe de estar en formato PDF y debe tener el tamaño del documento final.  

```
!![link.pdf]
```


### Listas númericas

Las listas ordenadas se identifican por los números seguidos de un punto y un espacio.

```
1. Primer elemento
2. Segundo elemento
3. Tercer elemento
```