# nivelacion

Valentina Gil Antía
   
Taller de Nivelación Curso Desarrollo Web Frontend 
 

1.	¿Qué es la lógica en el contexto de la programación? Y explicar por qué es importante en el desarrollo web Frontend.  

La lógica en programación es como el paso a paso para hacer algo en el computador. En Frontend, es clave para que la página se vea y funcione bien.

2.	Definir el concepto de “algoritmo” y proporcionar un ejemplo sencillo de un algoritmo relacionado con la lógica de programación. 
Un algoritmo es como una receta para hacer algo, es el paso a paso. Por ejemplo sumar dos números:
1. Meter número A
2. Meter número B
3. Sumar A y B
4. Mostrar el resultado

3.	¿Qué son estructuras de control en la programación?, ¿Cuáles son los tipos de estructuras de control y las estructuras más comunes de cada tipo?, Describir al menos dos tipos de estructura de control, explicar por qué son importantes y proporcionar ejemplos de cada uno de cómo se utilizan en el desarrollo web Frontend. 

Las estructuras de control dirigen cómo se ejecuta el programa. 
Los tipos son: secuenciales, condicionales y ciclos

Condicionales: decisiones (if, else), sirven para decidir qué hacer. Ejemplo: Mostrar un mensaje si el usuario está logueado.

Ciclos: repetir cosas (for, while) hasta que se cumpla una condición. Ejemplo: Pasar por una lista de compras para mostrar productos en una página web.




4.	Describir cómo se declaraban variables y constantes en JavaScript antes de la introducción de ECMAScript 6 (ES6). Explicar cómo ES6 mejoró la declaración de variables y constantes, y mencionar los problemas que esta mejora resuelve en el desarrollo web Frontend. 

Antes de ES6, declarar variables y constantes en JavaScript era menos claro, se usaba "var" para todo, y las constantes no existían como tal. ES6 mejoró eso con "let" y "const", dándonos más control y evitando problemas de alcance. En el Frontend, esto ayuda a evitar problemas con las variables y hace el código más claro.

5.	¿Cómo se declaran las funciones en JavaScript y cuál es la diferencia entre una declaración de función, una expresión de función y una función de flecha (arrow function)? Proporcionar ejemplos de cada una. 

Para declarar funciones en JavaScript, antes se tenía que usar "function". Con ES6, también tenemos funciones de flecha que son más cortas

Función tradicional: 
function sumar(a, b) {
  return a + b;
}

Función Flecha:
const multiplicar = (a, b) => a * b;

6.	¿Por qué es necesario el uso de funciones en el desarrollo web Frontend? Enumerar al menos tres razones fundamentales y proporcionar ejemplos de situaciones en las que las funciones son esenciales. Además, mencionar la ventaja de las funciones flecha en el contexto de estas razones. 

•	Las funciones nos ayudan a organizar el código, a hacerlo más fácil de entender. 
•	Permiten reutilizar código.
•	Evitan repetir lo mismo mil veces.

7.	¿Cuál es la diferencia entre parámetro y argumento? 
El parámetro es como el nombre de la variable que usamos en la función, mientras que el argumento es el valor real que le pasamos cuando llamamos a la función.
Parámetro: num1, num2
Argumento: 2, 4

8.	Definir el concepto de Callback y proporcionar un ejemplo práctico. 
Un Callback en JavaScript es básicamente una función que le pasamos como argumento a otra función. Esto permite ejecutar código de forma asíncrona, controlando el flujo del programa.

function hacerAlgo(despuesDeHacerAlgo) {
  console.log("Haciendo algo...");
  despuesDeHacerAlgo(); 
}

hacerAlgo(function() {
  console.log("Listo");
});

9.	¿Qué es el hoisting en JavaScript y cómo afecta a las variables y funciones? Proporcionar ejemplos de hoisting en declaraciones de variables y funciones. 

El hoisting en JavaScript es como una organización que hace que las declaraciones de variables y funciones se "muevan" arriba del código durante la ejecución. Ej:
console.log(variable1); 
var variable1 = "Hola";

Se interpreta así:
var variable1;
console.log(variable1); 
variable1 = "Hola";

10.	Definir brevemente el concepto de objeto en JavaScript y cuál es la visión general sobre este concepto. Indicar, también cómo se declaran estas estructuras de datos. 

Un objeto es como una caja que puede tener varios datos dentro.
Declaración:
const miObjeto = {
  clave1: valor1,
  clave2: valor2
}
11.	¿Qué son propiedades?, y ¿Cuál es la diferencia entre una propiedad y un método en un objeto? 

Las propiedades son como las cosas dentro de la caja (objeto). La diferencia entre propiedad y método es que un método es una función dentro del objeto.

12.	Explicar las dos formas de acceder a una propiedad de objetos e indicar las situaciones en que conviene usar una manera sobre la otra. 

Hay dos maneras de acceder a una propiedad de objetos. La primera es usando la notación de punto: const nombre = persona.nombre;
La segunda es usando la notación de corchetes: const nombre = persona["nombre"];

La primera es más común y fácil de leer, mientras que la segunda es útil cuando el nombre de la propiedad viene de una variable o cuando tiene espacios o caracteres especiales.

13.	¿Existe alguna forma de recorrer las propiedades de un objeto? En caso negativo, explicar por qué no es posible y en caso positivo proporcionar un ejemplo. Mencionar una situación en la cual sea muy útil recorrer las propiedades de un objeto. 

Sí, se puede recorrer las propiedades de un objeto con un bucle "for...in”. Ej:
var persona = {
  nombre: 'Valentina',
  edad: 22,
  ciudad: 'Medellín'
};

for (var propiedad in persona) {
  if (persona.hasOwnProperty(propiedad)) {
    console.log(propiedad + ": " + persona[propiedad]);
  }
}
Es útil cuando hay un montón de propiedades y se requiere hacer algo con cada una.

14.	¿Por qué son útiles los objetos en la programación web y qué tipos de datos pueden almacenar? 
Son útiles para organizar información, crear estructuras complejas y manipular datos de manera más fácil. 
Pueden almacenar datos simples como números o cadenas, pero también funciones, otros objetos e incluso arrays.

15.	¿Qué es un array en JavaScript y por qué son esenciales? 

Un array es como una lista de cosas en un mismo objeto. Son esenciales  porque permiten guardar múltiples datos bajo un solo nombre. Por ej: lista de productos en una tienda online. Cada producto puede ser un elemento del array.

16.	¿Cómo acceder a un elemento dentro de un array? Explicar con un ejemplo. 
Para acceder a un elemento en un array, usamos su índice. Hay que tener en cuenta que los índices empiezan en cero, así que el primer elemento es el 0, el segundo es el 1 y así sucesivamente.
const frutas = ["manzana", "banana", "uva"];
const segundaFruta = frutas[1];
console.log(segundaFruta); 
Este ejemplo imprime "banana" en consola. 

17.	Mencionar al menos tres funciones de arrays y describir su utilidad en la programación web. 

map(): Transforma cada elemento del array según una función que se le pase. Por ejemplo, duplicar cada número en un array.
filter(): Crea un nuevo array con solo los elementos que cumplan una condición. Sirve para filtrar datos específicos.
reduce(): Reduce el array a un solo valor aplicando una función acumuladora. Por ejemplo, sumar todos los elementos de un array.


18.	Proporcionar un ejemplo de cómo se utiliza una función de array para transformar y filtrar datos en un array. 
Este es un array de números y se van a filtrar solo los pares y duplicarlos:
const numeros = [1, 2, 3, 4, 5, 6];

const paresDuplicados = numeros
  .filter(numero => numero % 2 === 0) 
  .map(numero => numero * 2); 

console.log(paresDuplicados); 
En consola se imprime 4, 8, 12
 

MÓDULO SOBRE HTML, CSS Y RESPONSIVE DESIGN 
 
Preguntas teóricas 
 
1.	¿Qué significa HTML y cuál es su función en el desarrollo web? 

HTML significa "HyperText Markup Language". Es el lenguaje base para crear páginas web. Su función es estructurar el contenido de una página. Usa etiquetas para definir elementos como títulos, párrafos, imágenes y enlaces.

2.	¿Cuál es la estructura básica de un documento HTML? Describir las etiquetas esenciales.
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Título</title>
</head>
<body>

</body>
</html> 

Las etiquetas esenciales son:
<html> indica el inicio y fin del documento
<head> contiene información sobre el documento
<meta> especifica la codificación de caracteres y otros metadatos.
<title> define el título de la página
<body> contiene el contenido visible.

3.	¿Qué es CSS y cuál es su propósito en el desarrollo web? 

CSS es "Cascading Style Sheets". Su propósito es dar estilo y diseño a las páginas web. Permite cambiar colores, fuentes, márgenes, etc.

4.	¿Qué son selectores CSS, cuáles son los principales tipos de selectores y porqué es importante entender la especificidad en el contexto de las hojas de estilo en cascada (CSS)? Describir al menos tres tipos de selectores CSS y cómo la especificidad afecta a la aplicación de estilos en un proyecto de desarrollo web Frontend. Proporcionar ejemplos de situaciones en las que se utiliza la especificidad de selectores para resolver conflictos de estilos. 

Los selectores indican a qué elemento aplicarle los estilos. 
Selectores de Tipo: Seleccionan elementos por su tipo de etiqueta (ej: p para párrafos).
Selectores de Clase: Seleccionan elementos con una clase específica (ej: .boton).
Selectores de ID: Seleccionan un elemento con un ID único (ej. #encabezado).
La especificidad en CSS es clave para resolver conflictos al aplicarle estilos a la misma etiqueta. Cuanto más específico es un selector, más peso tiene. Ej: Selector de clase es más específico que de tipo. 



5.	Explicar las diferencias entre los estilos en línea (inline), estilos internos (embedded) y estilos externos (external) en CSS. Indicar cuál de los tres estilos es el recomendado usar y por qué.

En línea (style)
Interno (<style>) 
Externo (<link>)

Estas son formas de aplicar estilos en CSS. Se recomienda usar estilos externos para mantener el código más limpio y modular. Los estilos en línea afectan un elemento específico, los internos se aplican a la página entera y los externos permiten reutilizar estilos en múltiples páginas.
 
6.	¿Qué es flexbox y cómo se utiliza para el diseño de páginas web? 

Flexbox permite el diseño flexible en CSS. Ayuda a organizar elementos en una fila o columna con facilidad. Para usarlo hay que aplicar display: flex; al contenedor padre.

7.	Explicar cómo se emplean las propiedades flexbox y explicar la función de las principales propiedades en la creación de diseños flexibles. 

display: flex;: Activa el modo flex.
flex-direction: Determina la dirección de los elementos (fila o columna).
justify-content: Alinea los elementos en el eje principal (horizontal, vertical).
align-items: Alinea los elementos en el eje secundario.
flex: Define la capacidad de estiramiento de un elemento.


8.	¿Qué es CSS Grid Layout y en qué se diferencia de flexbox? 
CSS Grid Layout trabaja en dos dimensiones (filas y columnas), mientras que Flexbox opera en una dimensión.

9.	Proporcionar un ejemplo de cómo crear una cuadrícula sencilla con CSS Grid. 
.contenedor {
  display: grid;
  grid-template-columns: 50px 50px 50px;
  grid-template-rows: 150px 150px;
}

10.	¿Qué significa el diseño responsivo en el contexto del desarrollo web? 
Significa que la página se adapta a diferentes dispositivos y tamaños de pantalla, ya sea en un escritorio, tableta o celular. 

11.	Enumerar al menos tres técnicas o estrategias utilizadas para lograr el diseño responsivo en una página web.  

Media Queries: Usar reglas CSS para adaptar estilos según el tamaño de la pantalla.
Unidad em, vw, %: Usar unidades relativas para que los elementos se escalen en proporción al tamaño del contenedor padre.
Imágenes flexibles: Usar la propiedad max-width: 100%; en imágenes para que no se desborden de su contenedor y se ajusten a la pantalla.
 

MÓDULO SOBRE DOM E INTERACCIÓN CON EL DOM 
 
Preguntas teóricas 
 
1.	¿Qué es el DOM (Modelo de Objeto de Documento) en el contexto de la programación web? 

El DOM o Modelo de Objeto de Documento, es básicamente la versión estructurada y manipulable de la página web (como un esqueleto interactivo).

2.	¿Cuál es la diferencia entre el DOM y el HTML en una página web? 

El HTML define la estructura, y el DOM toma esa estructura y la convierte en algo que se puede mover y cambiar.

3.	¿Por qué es importante entender y manipular el DOM en el desarrollo web Frontend? 

Porque eso es lo que permite que la página sea dinámica (actualizar, agregar o quitar elementos).

4.	¿Qué son los eventos del DOM y cuál es su función en una página web? 

Son acciones o sucesos que ocurren (como hacer clic, enviar un formulario o cargar la página).

5.	Proporcionar ejemplos de eventos prácticos y comunes, como “click”, “submit” y “load o DOMContentLoad”. 

click: Cuando se hace clic en algo.
submit: Se desata cuando se envía un formulario.
load o DOMContentLoaded: se dispara cuando el DOM ha cargado completamente.

6.	¿Por qué es importante manejar eventos en la interacción usuario-web y cómo se añaden controladores de eventos a los elementos del DOM? 

Es importante porque le da vida a la interacción usuario-web, permite que la página web responda dinámicamente a las acciones del usuario.

7.	Describir al menos tres métodos para seleccionar elementos del DOM en JavaScript.

getElementById: selecciona usando ID.
getElementsByClassName: selecciona usando la clase.
querySelector: se puede escoger selector.
 
8.	¿Cómo se crea un nuevo elemento HTML y se agrega al DOM utilizando JavaScript? 

Esto implica crear un nuevo objeto de elemento, configurar sus propiedades según sea necesario, y luego agregar ese elemento a un elemento existente en el DOM.

9.	¿Cuál es la importancia de la manipulación del DOM en la creación de aplicaciones web dinámicas e interactivas? 

Manipular el DOM implica cambiar el contenido en tiempo real y actualizar elementos sin recargar toda la página lo cual da vida a la experiencia del usuario

10.	Explicar brevemente los conceptos “event bubbling” y “event delegation” en el contexto de eventos del DOM. 

Event bubbling es el comportamiento en el que un evento se propaga desde el elemento objetivo hasta el elemento raíz del DOM.
Event delegation implica asignar un controlador de eventos a un padre de varios elementos en lugar de asignarlo a cada elemento individual.

11.	¿Por qué son relevantes los conceptos “event bubbling” y “event delegation” en la gestión de eventos en páginas web con múltiples elementos interactivos? 

Estos conceptos son valiosos en páginas web con muchos elementos interactivos, ya que ayudan a optimizar el rendimiento y a escribir código más eficiente.
 

MÓDULO SOBRE COMUNICACIÓN CON EL SERVIDOR (STORAGE, PROMESAS, ASINCRONÍAS Y PETICIONES HTTPS) 
 
Preguntas teóricas 
 
1.	Definir brevemente el concepto de localStorage y sessionStorage.  

Son formas de almacenar información en la computadora del usuario para que la página web pueda recordar cosas la próxima vez que se visite.

2.	Describir las diferencias claves entre localStorage y sessionStorage. 

La gran diferencia entre ellos es que localStorage guarda la información sin límite de tiempo, mientras que sessionStorage solo mantiene los datos durante la sesión actual del navegador.

3.	¿Por qué son útiles para almacenar datos en el navegador y cuál es su límite de capacidad? 

Son útiles porque permiten que las páginas web guarden datos de manera eficiente y rápida.

4.	¿Qué son las promesas en JavaScript y para qué se utilizan en el desarrollo web? 

Las promesas en JavaScript son como acuerdos entre el código y operaciones que pueden llevar tiempo, como cargar imágenes o hacer solicitudes a un servidor. 
Se usan para mantener el código ordenado y eficiente al manejar operaciones asincrónicas de manera más legible, en lugar de bloquear el flujo del programa.

5.	Explica el concepto de asincronía en programación y cómo las promesas ayudan a manejar operaciones asincrónicas. 
La asincronía en programación se refiere a la ejecución de tareas sin tener que esperar a que una tarea anterior se complete.

6.	Proporciona un ejemplo de cómo se utiliza una promesa para realizar una operación asincrónica, como una solicitud de red. 

function hacerSolicitud() {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      const exito = true; 
      if (exito) {
        resolve('Solicitud exitosa.');
      } else {
        reject('Error.');
      }
    }, 2000);
  });
}

hacerSolicitud()
  .then((respuesta) => {
    console.log(respuesta);
  })
  .catch((error) => {
    console.error(error);
  });


7.	¿Qué es JSON Server y cómo se utiliza en el desarrollo web? 
JSON Server es una herramienta que permite crear rápidamente una API REST simulada a partir de un archivo JSON. 

8.	¿Por qué es útil simular una API REST falsa con JSON Server en el desarrollo frontend? 
Esto es útil en el desarrollo web para probar y simular interacciones con una API antes de tener una implementación real sin necesidad de depender de un backend.

9.	¿Cuáles son las diferencias claves entre los métodos del objeto promesa .then().catch() y las palabras claves async/await? 

.then().catch() es una forma más antigua y utiliza callbacks para manejar el resultado o los errores de una promesa, mientras que async/await proporciona una sintaxis más estructurada, permitiendo que el código se asemeje más a un estilo síncrono, facilitando su comprensión.

10.	Proporciona un ejemplo de cómo configurar una API falsa con JSON Server y realizar solicitudes (GET, POST, PUT, PATCH y DELETE) a través de ella. 

Configurar una API falsa con JSON Server implica crear un archivo JSON que actúa como base de datos y ejecutar el servidor con el comando json-server. Luego se pueden hacer solicitudes HTTP a través de la aplicación.

11.	Describe las diferencias entre Fetch y Axios como métodos para realizar solicitudes HTTP en JavaScript. 

Fetch es una función nativa del navegador que proporciona una interfaz para realizar peticiones HTTP, mientras que Axios es una biblioteca externa que simplifica el proceso y tiene características adicionales.

12.	¿Por qué es importante considerar las peticiones HTTP en aplicaciones web modernas? 

Porque permiten la comunicación entre el frontend y el backend, facilitando la obtención y actualización de datos de forma asincrónica.

13.	Proporciona ejemplos de cómo se utilizan Fetch y Axios para realizar solicitudes GET y POST. 

Para realizar solicitudes GET y POST, tanto con Fetch como con Axios, el proceso es similar en términos de objetivo pero difiere en la sintaxis
Con Fetch, se utiliza la función fetch() donde se especifica la URL y el método de solicitud (GET o POST) y la respuesta se maneja con promesas. 
Axios, se utiliza axios.get() especificando la URL, y para una solicitud POST, axios.post() con la URL y los datos a enviar.

14.	Explica la importancia del manejo de errores al trabajar con promesas en el desarrollo web. 
El manejo de errores en las promesas es esencial para mantener la estabilidad y seguridad de las aplicaciones.

15.	Describe cómo se manejan los errores en las promesas, incluyendo el uso de catch. 

Manejar los errores en las promesas implica registrar el error para el seguimiento y análisis, notificar al usuario de manera adecuada o incluso intentar recuperar la operación.
Catch se encarga de atrapar cualquier error que ocurra durante la ejecución de la promesa.

16.	¿Cuáles son las diferencias claves entre los métodos del objeto promesa .then().catch() y la estructura try/catch? 

.then().catch() es específico para promesas y se utiliza para encadenar operaciones en caso de éxito (.then()) y gestionar errores (.catch()). En cambio, try/catch es más general y se extiende a cualquier bloque de código. 

17.	Proporciona un ejemplo de cómo se puede manejar un error en una promesa al realizar una solicitud de red. 

fetch('https://api.com/apli')
  .then(response => {
    if (!response.ok) {
      throw new Error('La solicitud no fue exitosa');
    }
    return response.json();
  })
  .then(data => {
  })
  .catch(error => {
    console.error('Error de red:', error.message);
  });

 

MÓDULO SOBRE REACT JS 
 
Preguntas teóricas 
 
1.	Explicar brevemente el concepto de ReactJS y sus principales características.
Es una biblioteca de JavaScript que se utiliza para construir interfaces de usuario interactivas y eficientes. Su principal característica es un enfoque basado en componentes, mejoramiento del rendimiento.
 
2.	Definir qué es un componente en ReactJS y mencionar los tipos de componentes que existen. 

Un componente es una pieza reutilizable e independiente de la interfaz de usuario.

3.	¿Qué es el Virtual DOM y cuál es su función en ReactJS? 

Es una representación virtual y eficiente del DOM real. Actúa como un intermediario entre el estado actual y el DOM, permitiendo actualizaciones.

4.	¿Qué es JSX en ReactJS y porqué es importante? 
Es extensión de la sintaxis de JavaScript que permite escribir código similar a HTML dentro de archivos de JavaScript (integrando HTML en el código JavaScript).

5.	¿Qué es un Hook en ReactJS y cuál es su propósito? 

Es una función especial que permite a los componentes de función acceder al estado y a las características del ciclo de vida de los componentes de clase.

6.	Mencionar al menos tres tipos de Hooks en ReactJS y explicar brevemente para qué se utilizan. 

useState: Permite a los componentes de función tener estado local.
useEffect: Se utiliza para ejecutar código después de que un componente se monta, actualiza o desmonta.
useContext: Facilita el acceso al contexto de React dentro de un componente de función.


7.	¿Cuáles son las reglas de uso para los Hooks en ReactJS? 

Las reglas de uso para los Hooks en ReactJS incluyen llamar a los Hooks solo en el nivel superior del componente de función, no llamarlos en loops, condiciones o funciones anidadas.

8.	Explicar qué es React Router DOM versión 6, para qué se utiliza y cuáles son sus principales componentes y Hooks. 

React Router DOM versión 6 es una librería de enrutamiento para React que facilita la navegación y gestión de las URL en una aplicación de una sola página. Sus principales componentes son BrowserRouter, Route, y Link y sus Hooks principales son useNavigate, useParams.

9.	Explicar cómo se realiza la navegación entre diferentes páginas utilizando React Router DOM. 
La navegación entre diferentes páginas utilizando React Router DOM se realiza mediante el componente Link, que crea enlaces de navegación. También se puede utilizar el Hook useNavigate para realizar navegación programática (cambiar de página mediante código en vez de acciones del usuario).

10.	¿Cómo se definen rutas en React Router DOM? 

Las rutas en React Router DOM se definen mediante el componente Route

11.	Describir cómo crear un proyecto ReactJS con Vite 
Hay que instalar vite con el código: npx create-vite nombre-app --template react y luego entrar a la carpeta del proyecto. 

12.	Describir cómo desplegar un JSON server en cualquier Hosting free o servicio en la nube gratuito de su elección 

Hay que crear un repositorio en Github y subir el código, luego conectar la cuenta de por ejemplo Vercel y allí importar el proyecto de Github. 


13.	Describir cómo desplegar una aplicación en cualquier Hosting de su elección.
Hay que crear el repositorio en Github y subir el código, luego conectar la cuenta de Github con Netlify, importar el proyecto y revisar la url de despliegue.
 
 

MÓDULO SOBRE GESTION DE ESTADOS Y DATOS CON REACT CONTEXT Y 
USEREDUCER 
 
Preguntas teóricas 
 
1.	¿Qué es React Context y para qué se utiliza en el desarrollo web con React? 

Es una característica de React que facilita la gestión del estado y la propagación de datos en toda la aplicación sin pasar props a través de cada nivel de componente. Se utiliza para compartir información, como el idioma o el estado global, entre componentes sin la necesidad de pasar manualmente estas propiedades entre cada componente en la jerarquía.

2.	Describir cómo se crea un contexto en React y cómo se proporciona y consume información a través de él. 

Para crear un contexto en React, primero se define el contexto utilizando createContext y luego se proporciona un proveedor que envuelve los componentes que necesitan acceder a esa información.

3.	¿Cuál es la ventaja de utilizar React Context en lugar de pasar props a través de múltiples componentes? 

Al evitar pasar props a través de múltiples niveles de componentes, el código se vuelve más legible y mantenible. También ayuda el  "prop drilling” (los componentes intermedios reciben y pasan props que no necesitan utilizar).

4.	Explicar el propósito de useReducer en React y cómo se diferencia de useState. 

useReducer se usa para gestionar estados complejos en aplicaciones React. A diferencia de useState, que es más adecuado para estados simples.

5.	Describe los argumentos que toma la función useReducer. 
La función useReducer toma dos argumentos principales:
Reducer Function: define cómo el estado debe cambiar en respuesta a una acción. 
Initial State: Este es el estado inicial que se establece al inicio. 

6.	¿Por qué es útil utilizar useReducer para gestionar el estado en aplicaciones más complejas? 

El patrón de useReducer centraliza la lógica de actualización del estado en un solo lugar (el reductor), facilitando el mantenimiento y la comprensión del código.

7.	¿Cómo se puede utilizar React Context junto con useReducer para gestionar el estado global en una aplicación de React? 

Crear un contexto que utilice useReducer como método para gestionar el estado permite que múltiples componentes accedan y actualicen el mismo estado global de manera coherente.

8.	¿Por qué es importante tener un sistema de gestión de estado global en aplicaciones React más grandes? 
Esto es esencial para garantizar coherencia, accesibilidad global y facilitar la comunicación entre componentes sin depender de relaciones directas.

9.	Menciona al menos tres ventajas de utilizar una combinación de React Context y useReducer en comparación con el manejo de estado local en componentes. 
•	Reducción del prop drilling
•	Eficaz manipulación de acciones asincrónicas 
•	Mayor escalabilidad.

10.	¿En qué situaciones podría ser beneficioso migrar de un enfoque de manejo de estado local a un enfoque de estado global utilizando React Context y useReducer? 

Puede ser beneficioso en situaciones donde la complejidad de la aplicación aumenta, la necesidad de compartir estado entre componentes es frecuente y se busca una solución más organizada.
 
 
 
 
