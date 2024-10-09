
# Respuestas sobre XML

### 1. Características propias del lenguaje XML
- **XML** (Extensible Markup Language) es un lenguaje de marcado flexible diseñado para almacenar y transportar datos de manera estructurada.
- No tiene etiquetas predefinidas, lo que permite definir etiquetas personalizadas.
- Es legible tanto por humanos como por máquinas, facilitando el intercambio de datos entre sistemas heterogéneos.
- Los documentos XML deben ser bien formados y cumplir con una estructura jerárquica clara, como un árbol de nodos.

### 2. Estructura de un documento XML y reglas sintácticas
- Todo documento XML tiene un **elemento raíz** que contiene todos los demás elementos.
- Cada elemento debe estar delimitado por etiquetas de apertura y cierre.
- Las etiquetas deben estar correctamente anidadas, sin solapamientos.
- Los atributos deben ir entre comillas.
- Un documento XML debe incluir una **declaración XML** que especifique la versión y la codificación.

### 3. ¿Qué es un nodo raíz en XML?
El **nodo raíz** es el elemento principal del documento XML. Todos los demás elementos están anidados dentro de este. Solo puede haber un nodo raíz por documento. Por ejemplo:

```xml
<persona>
  <nombre>Juan</nombre>
</persona>
```
En este caso, `persona` es el nodo raíz.

### 4. ¿Qué es un elemento vacío? Ejemplos
Un **elemento vacío** es aquel que no contiene texto ni elementos hijos. Se puede escribir de dos formas:
- `<etiqueta></etiqueta>`
- `<etiqueta/>`

Ejemplo:
```xml
<nombre></nombre>
<nombre/>
```
Ambas formas representan un elemento vacío.

### 5. ¿Qué sentido tiene crear documentos XML bien formados?
Un documento XML bien formado sigue todas las reglas sintácticas del lenguaje, lo que asegura que puede ser interpretado correctamente por cualquier sistema o aplicación que lo procese. Además, facilita su validación y reutilización en diferentes contextos.

### 6. ¿Qué es un espacio de nombres? Ventajas de uso
Un **espacio de nombres** en XML es una forma de evitar conflictos de nombres cuando se utilizan etiquetas que podrían tener el mismo nombre pero pertenecen a diferentes contextos. Esto se logra mediante el uso de **URI** o prefijos específicos. Ventajas:
- Permite combinar vocabularios de diferentes esquemas XML sin ambigüedades.
- Mejora la claridad y organización en documentos complejos.

### 7. Entidades en XML
Las **entidades** son una forma de representar caracteres especiales o secuencias de texto en XML. Por ejemplo:

```xml
<mensaje>El símbolo mayor que es &gt;</mensaje>
```
En este ejemplo, `&gt;` es una entidad que representa el símbolo `>`.

### 8. Comentarios en XML
Los comentarios en XML se escriben entre `<!--` y `-->`. Por ejemplo:

```xml
<!-- Este es un comentario -->
<persona>
  <!-- Nodo raíz del documento -->
  <nombre>Juan</nombre>
</persona>
```
Es importante recordar que no se pueden incluir dos guiones seguidos `--` dentro de un comentario, ya que esto generaría un error.

