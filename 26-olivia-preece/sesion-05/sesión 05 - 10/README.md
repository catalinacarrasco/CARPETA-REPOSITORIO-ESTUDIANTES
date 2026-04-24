# sesión 05 - 10/04

***CLASE 24/04***

* Para agregar un código en github hay que agregar tres comillas (ej: '''rect(10,10,30,100)''' ) Para bloque de código
* Para usar entre medio de una oración 'código p5'

**CLASE DE HOY**  
4 pilares fundamentales

**DESCOMPOSICÓN**  
"Dividir para conquistar"  
Consiste en tomar un problema grande y complejo y romperlo en partes pequeñas y manejables.  
* En diseño: Si quieres visualizar la "Brecha Salarial" no programes todo de una vez, separar o diseñar primero "sueldo A", luego "saldo B", "C", después interacción y luego por último el fondo
* En el código: Se traduce en el uso de **funciones propias**

**RECONOCIMIENTO DE PATRONES**  
"Encontrar similitudes"  
Es observar tendencias o regularidades dentro de un problmea. Si algo se repite o sigue una logica constante, podemos automatizarlo.  
* Diseño: Para presentar 100 personas no necesitas deobujar 100 veces. Notas que todas son un c{irculoo con una posicion x distinta.
* Código: Bucles

**ABASTRACCIÓN**  
"Lo importante v/s el detalle"  
Filtrar info necesaria y quedarse solo con las caracteristicas que definen el problema. Es crear una representaci{on simbolica de la realidad.  
* En diseño: Simplificar formas de representación
* Uso de variables y funcion map()

**ALGORITMO**  
"La receta paso a paso"  
Diseño de una serie de reglas ordenadas para resolver un problema. Es el "plan de acción" que debe seguir el sistema.  
* diseño: Flujo de la experiencia  
* código: Se traduce en el diagrama de flujo y en las condicionales (if/else)

Vamos a tener en p5 dos tipos de interacci{on  
* Interacción discreta (eventos)
cuando ocurre un evento especifico (clic) y el sistema responde con una acción única (aparecen círculos). Es un in

### **FUNCIONES PROPIAS** ###  
Importante para dar:  
1. Modularidad
2. Reusabilidad
Para simplificar la contrucción del código y reutilizar las funciones.

**Cómo va a ir escrito**  
Función abajo va a ir function(){  
sintaxis function Nombredelafunción()}  
Ejemplo: (abajo de function draw)
Function Dibujarfiguras()}  
stroke()  
strokeWeight()
fill()  
ellpise()

'''

let x=0  
let y=0  
let speed = 3;  
function setup() {  
createCanvas(400, 400);  
}  
function draw() {  
background(255, 111, 0);
    noStroke();
  fill(24, 84, 61);
  ellipse(x,200,100,100);'//cordenada x va a ser variable x, luego y(200) y de 50x50'
  x=x+speed '//avanza de tres pixeles cada vez que hace el draw (spped =3)'
   if (x > width || x < 0) {
    print("fueradecuadro")
speed = speed * -1; '// pelota avanza por sus valores negativos (cualquier cosa multiplicada por -1)'
}
  noStroke();
  fill(173, 217, 199);
  ellipse(200,y,50,50);'//cordenada x va a ser variable x, luego y(200) y de 50x50'
  y=y+speed
  if (y > width || y < 0) { '//condicional siempre llave que abre y cierra'
    print("fueradecuadro")
    speed = speed *-1; 
}
  } '// ultima llave que cierra el darw'
  
  '''

