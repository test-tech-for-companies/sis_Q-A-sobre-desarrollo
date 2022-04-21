# Q&A sobre desarrollo

----
1. ¿Quién creó el lenguaje de programación de Python?
```
Guido van Rossum
```
----
2. ¿Qué pasa cuando escribes? `gcc main.c`
```
el comando `gcc main.c` realiza una serie de fases con el objetivo de obtener un archivo binario que pueda correr en el sistema operativo

El proceso es el siguiente:
1. El programador escribe un código fuente para resolver un problema (archivo main.c).
2. A través del comando gcc se da la orden de iniciar este proceso que termina con la ejecución del archivo.
3. Preprocesador: expande el código fuente
4. Compilador: convierte el código expandido en código ensamblador.
5. Ensamblador: convierte el código de ensamblaje en código de objeto.
6. Linker: vincula el código de ensamblaje a las bibliotecas para crear código de objeto.

El archivo ejecutable está listo.
```
----
3. ¿Cuál es el propósito de 'if __name__ '==' __main __ ': `en Python?

```
Cuando un intérprete de Python lee un archivo de Python, primero establece algunas variables especiales. Luego ejecuta el código desde el archivo. Una de estas variables es `__name__`.

Los archivos de Python se llaman módulos y se identifican mediante la extensión de archivo .py.

Entonces, cuando el intérprete ejecuta un módulo, el variable __name__ se establecerá como __main__ si el módulo que se está ejecutando es el programa principal.

Pero si el código está importando el módulo desde otro módulo, entonces el variable __name__ se establecerá en el nombre de ese módulo.
```

----
4. ¿En Python, Que es el metodo `__init__` ?
```
El método __init__ es un método especial de una clase en Python. El objetivo inicializar los atributos del objeto que creamos.

* El método __init__ es el primer método que se ejecuta cuando se crea un objeto.
* El método __init__ se llama automáticamente. Es decir es imposible de olvidarse de llamarlo ya que se llamará automáticamente.

```
----
5. ¿Cuál es la diferencia entre una clase y un “objeto o instancia”?
```
Una clase es una plantilla para la creación de objetos de datos según un modelo predefinido. En ella se define un conjunto de variables (el estado), y métodos apropiados para operar con dichos datos (el comportamiento).

Instanciar objetos es el proceso de generar un ejemplar de una clase, es decir, la clase es como una declaración de una forma y el objeto es un caso o elemento concreto que responde a esa forma.
```
----
6. ¿Explique cómo funciona lo siguiente:
res.file ? jumpLis() : sap()

```c
condition ? condition_if_true : condition_if_false
```

```
Es una expresion condicional de una línea. En este caso
* Si existe el archivo res ejecuta el método jumpList() y si no ejecutará el método sap()
```

----
7. ¿Qué es mutable e inmutable?
```
En Python, todo es un objeto. Un objeto tiene su propio estado interno. Algunos objetos le permiten cambiar su estado interno y otros no.

Un objeto cuyo estado interno se puede cambiar se denomina objeto mutable, mientras que un objeto cuyo estado interno no se puede cambiar se denomina objeto inmutable.

Los siguientes son ejemplos de objetos inmutables.
Recordemos inmutable significa que no puede ser cambiado despues de ser creado:

1. Numbers
2. String
3. Tuples

Y los siguientes son ejemplos de objetos mutables
Recordemos los valores del objecto puede cambiar en cualquier momento después de su creación:

1. Lists
2. Sets
3. Dictionaries
```
----
8. ¿Cuál es el significado de sobrescribir un método en Programación Orientada a Objetos?
```
Por sobreescribir métodos se considera que desde una clase heredada, se define un método que se llama igual que otro de la clase padre, de este modo cuando lo invocamos desde un objeto al que llamamos, es al de la clase hijo, haciendo que se ejecute ese código.
```
----
9. ¿Qué es un shell?
```
Un shell, es un interprete de comandos (interfaz). Es decir, un programa que se encarga de traducir los comandos del usuario, a instrucciones para acceder a los servicios del sistema operativo.
```
----
10. ¿Cuál es la diferencia entre un terminal y una shell?
```
Un terminal es un entorno donde entran y salen textos. Cuando una terminal es física, adquiere el nombre de consola. Y Shell será quien interprete los datos y comandos que envía el terminal.
```
----
11. ¿Cuál es la diferencia entre un hard link y un symbolic 
link en linux?
```
* Los enlaces simbólicos se pueden hacer con ficheros y directorios mientras que los duros solo entre ficheros.
* Los enlaces simbólicos se pueden hacer entre distintos sistemas de ficheros, los duros no.
* Los enlaces duros comparten el número de inodo, los simbólicos no.
* En los enlaces simbólicos si se borra el fichero o directorio original, la información se pierde, en los duros no.
* Los enlaces duros son copias exactas del fichero mientras que los simbólicos son meros punteros o «accesos directos».
```
----
12. ¿En Python si quisiera usar datos que luego de su creación no “se puedan cambiar” que estructura de datos usaría?

```
Tuples: una colección de objetos inmutable
```
----
13. ¿Cuál es la diferencia entre git y github?

```
Git(software de control de versiones) se refiere al proceso de guardar diferentes archivos o «versiones» a lo largo de las diferentes etapas de un proyecto.
GitHub es una plataforma basada en la web que incorpora las características de control de versiones de git para que puedan ser utilizadas de forma colaborativa.
```

----
14. ¿Qué es una cola “queue” y cómo funciona?
```
Una cola es una estructura de datos, caracterizada por ser una secuencia de elementos en la que la operación de inserción push se realiza por un extremo y la operación de extracción pull por el otro. También se le llama estructura FIFO (del inglés First In First Out), debido a que el primer elemento en entrar será también el primero en salir.
```
----
15. ¿Qué es un método estático?
```
Los métodos estáticos no requieren la creación de objetos de una clase para ser llamados, se pueden llamar dirigidos a la clase. Esto es diferente de un método de clase normal, que requiere la iniciación del objeto y se llama en el objeto.
```
----
16. ¿Hablando de C o C++, Sabe qué es un puntero?
```
Un puntero no es más que una variable estática cuyo contenido es una dirección de memoria de otra variable. El propósito del puntero es ahorrar espacio en la memoria y lograr un tiempo de ejecución más rápido.
```
----
17. ¿Cuál es la diferencia entre los módulos y los paquetes en Python?
```
Un módulo es un archivo de Python cuyos objetos (funciones, clases, excepciones, etc.) pueden ser accedidos desde otro archivo. 
Un paquete es una carpeta que contiene varios módulos.
```
----
18. ¿Cuáles son las palabras clave para cambiar el nombre de una columna durante una consulta SQL?
```sql
SELECT nombre_original AS nuevo_nombre_que_ponemos FROM tabla;
```
```
Usamos alias con AS
```
----
19. ¿Nombre una alternativa de software a Haproxy como balanceador de carga?

```
Neutrino
```

----
20. ¿Explique cuál es el papel principal de un balanceador de carga?

```
El balanceador de carga ayuda a los servidores a mover los datos de manera eficiente, optimiza el recurso de entrega de aplicaciones y evita las sobrecarga de los servidores. Un balanceador iguala el trabajo del mismo para que las aplicaciones respondan eficazmente.  
```
----
21. ¿Qué es Nginx?
```
El software del servidor es conocido como un servidor web de alto rendimiento que puede servir simultáneamente al mayor número posible de clientes web, sin consumir muchos recursos. Adicionalmente tiene otras funciones asociadas como:
* Proxy inverso: le permite usar NGINX como un proxy inverso (HTTP, TCP, UDP) para acelerar las carga en la web o usar un proxy de e-mail (IMAP, POP3, SMTP).
* Cifrado TLS: permite el intercambio seguro de datos.
* Gestión de ancho de banda: asocia la banda ancha ideal para cada servicio ofrecido.
* Equilibrio de carga: distribuye solicitudes para descargar el servidor central.
* Videostreaming: ofrece un alto rendimiento para streaming de archivos MP4 y FLV.
```
----
22. ¿Cuál es la diferencia entre una cola y una pila?

| Pila | Cola |
| -------- | -------- |
| Los objetos son insertados y retirados en el mismo extremo.  |Los objetos se insertan y extraen desde distintos lados.|
| En pilas sólo se utiliza un puntero. Se apunta a la parte superior de la pila. | En las colas, dos punteros diferentes se utilizan para extremos delantero y trasero. |
| En pilas, el último objeto insertado es el primero en salir. | En las colas, primero se elimina el objeto insertado en primer lugar. |
| Pilas siguen último en entrar, primero en salir fin (LIFO). | Colas siguiente First In First Out orden (FIFO). |
| operaciones de la pila se llaman push y el pop. | operaciones de la cola son llamadas enqueue y dequeue. |
| Colección de platos de la cena en una boda es un ejemplo de pila. | La gente que estaba en un archivo para subir a un bus es un ejemplo de cola. |

----
23. Graphql en sus palabras que ventajas tiene?, y si hablamos de Angular o React con graphql que librerías a manejado, y si hablamos de backend que librerías a manejado?
----
24. Usted prefiere usar API REST o GRAPHQL y porque?
```
Yo preferiría usar GRAPHQL me permite mayor alcance al conjunto de datos que quiero obtener. Se adapta a las necesidades utilizando el lenguaje de consulta de GraphQL (basado en Schemas) describiendo lo que le gustaría tener como respuesta, así como combinar diferentes entidades (o tipos) en una consulta y qué atributos.
```
----
25. Solo si ya tiene experiencia en Graphql conteste: como obligar la recarga de la cache de
graphql sin usar un refresh?
```
N/A
```
----
26. A trabajado con RJSX? Y si lo a echo para que es esta librería?
```
N/A
```
----
27. Que es un observable?
----
28. Que es un BehaviorSubject?
----
29. Nombre que Bases de Datos SQL y No-SQL a manejado? Y su auto calificación para cada una de ellas, como ejemplo: mariadb-Basico, Dynamo-Experto etc.

* Postgres: Medio
* Mysql:  Medio
* Mongo: básico
* Dynamo: bajo
----
