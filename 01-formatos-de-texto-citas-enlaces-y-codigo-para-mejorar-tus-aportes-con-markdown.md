
_Anterior:_ ⏪ [_✍️💡 Escribe textos geniales con Markdown 👨‍🎨👩‍🎨_][url-indice]


## 📖 Formatos de texto, citas, enlaces y código para mejorar tus aportes


Las etiquetas de énfasis, permiten resaltar parte del texto sin obligar un salto de línea.


==«==
---
* `*Este texto aparecerá en cursiva*`
 `_Este texto también aparecerá en cursiva_`
 `**Este texto aparecerá en negrilla**`
 `__Este texto también aparecerá en negrilla__`
 `~~Este texto aparecerá tachado~~`
 `_**Puedes** combinarlos_`
 `También puedes ==resaltarlos==`


==» El código anterior producirá: »==
---


* *Este texto aparecerá en cursiva*
 _Este texto también aparecerá en cursiva_
 **Este texto aparecerá en negrilla**
 __Este texto también aparecerá en negrilla__
 ~~Este texto aparecerá tachado~~
 _**Puedes** combinarlos_
  También puedes ==resaltarlos==
 
## 📑 Citas

Las citas se inician con el símbolo >. También se suele colocar en cursiva el párrafo entre comillas y en el renglón siguiente el autor de la cita. Algunas implementaciones de Markdown eliminan algunas ciertas para evitar inyección de código Sql, aquí recuperamos los espacios arriba y abajo de la cita usando un renglón con texto resaltado  (cualquier texto debe servir) y seguido un renglón contres guiones al medio, el cual convierte en encabezado el renglón superior y proporciona los espacios perdidos.

==«==
---


````> _**“ Los hombres sabios hablan porque tienen algo que decir; los necios porque tienen que decir algo. ”**_`
`>>Platón````


==» El código anterior producirá: »==
---

>  _**“ Los hombres sabios hablan porque tienen algo que decir; los necios porque tienen que decir algo.  ”**_
> Platón.


## 🔗 Enlaces
Los enlaces se pueden insertar copiando y pegando la URL completa (no recomendado por falta de legibilidad) o siguiendo la siguiente regla: El texto alternativo para el enlace entre corchetes cuadrados seguido de la URL dentro de paréntesis.


==«==
---

`http://platzi.com – enlace creado de forma automática!`
`[Platzi](http://platzi.com)`


==» El código anterior producirá: »==
---

http://platzi.com – enlace creado de forma automática!

[Platzi](http://platzi.com)

## 📜 Encabezados
Para usar la etiqueta de encabezados, deberás iniciar la línea de texto con dos caracteres ##, así:


==«==
---

`## Este es un encabezado`


==» El código anterior producirá: »==
---

## Este es un encabezado
> 

En Platzi la etiqueta H1 se encuentra reservada por el sistema para mantener una correcta estructura semántica. Rara vez necesitarás encabezados diferentes al H2.


## 🔪 Separadores o saltos de línea

Para incluir una espacio de separación entre párrafos deberás, párrafos usar un doble salto de línea. Cuando deseas incluir una línea de separación puedes intentar con tres guiones al medio seguidos.

==«==
---


`Renglón anterior.`
`---`
`Renglón siguiente.`


==» El código anterior producirá: »==
---

==«==
---
Renglón anterior.
---
Renglón siguiente.


==«==
---

`Renglón anterior.`
`==»==`
`---`
`Renglón siguiente. `


==» El código anterior producirá: »==
---



Renglón anterior.
==»==
---
Renglón siguiente. 



![Imgur](https://i.imgur.com/X2TrK4G.jpg) 
>## Metodo alternativo
>**Si la etiqueta anterior deja una separación muy pequeña, intenta utilizando alguna de estas dos imágenes siguientes. Elige la que mejor te funcione.**
>==«==
>---
>Salto de línea (insertando imagen en blanco)
>Renglón anterior
`![Imgur](https://i.imgur.com/X2TrK4G.jpg)`
Renglón medio
`![Imgur](https://i.imgur.com/EG1jOdW.jpg)`
Renglón siguiente
>
>==» El código anterior producirá: »==
>---
>Renglón anterior. (Este texto se incluye como referencia para medir el tamaño del separador)
![Imgur](https://i.imgur.com/EG1jOdW.jpg)Renglón medio
![Imgur](https://i.imgur.com/EG1jOdW.jpg)
Renglón siguiente
O también puedes usar esta otra técnica
--

==«==
---

Renglón anterior.
`![url1](https://via.placeholder.com/1x1/f6f6f6/f6f6f6?text=+)`
Renglón siguiente. 


==» El código anterior producirá: »==
---
Renglón anterior.
![url1](https://via.placeholder.com/1x1/f6f6f6/f6f6f6?text=+)
Renglón siguiente. 


## 🖥️ Sintaxis para incluir código
==«==
---

\`Una sola línea de código\`


==» El código anterior producirá: »==
---


`Una sola línea de código`


También puedes incrustar bloques de código de varias líneas: 

==«==
---
````
\````javascript
function fancyAlert(arg) {

    if(arg) {

    $.facebox({div:'#foo'})

    }
}
\````
````

==» El código anterior producirá: »==
---


````javascript
function  fancyAlert(arg) {
    if(arg) {
    $.facebox({div:'#foo'})
    }
}
````

## 🏃🏽‍♀️ Escapar caracteres

==«==
---

Para escapar caracteres deberás usar el símbolo \ (barra invertida) justo antes del carácter que se quiere escapar.

`- [ ] \(Si vas a incluir paréntesis después de corchetes cuadrados) será necesario escapar el primer paréntesis`


==» El código anterior producirá: »==
---


 - [ ] \(Si vas a incluir paréntesis después de corchetes cuadrados) será necesario escapar el primer paréntesis.

**Será necesario hacer esto cuando quieras que alguno de los siguientes caracteres de control sea mostrado en el documento.**

```
\  barra invertida
`  tilde invertida
*  asterisco
_  guión bajo
#  numeral o almohadilla o gato (o como lo llames 😉)
+  símbolo de suma
-  guión
.  punto
!  exclamación
{} llaves
[] corchetes
() paréntesis
```  






==«==
---



Para evitar que la creación automática de enlaces, deberás escapar parte de sus caracteres así:

`https\:/[]()/example.com/`

==» El código anterior producirá: »==
---
https\:/[]()/example.com/


==«==
---

**_Continúa tu aprendizaje con:_**

* 📷 [_Integrar imágenes en tus comentarios o tutoriales_][url-imagenes] ⏩

==»==
---



[📖][url-textos] [📷][url-imagenes] [🎬][url-animaciones] [🍕][url-emojis] [🆎][url-variables] [🔲][url-botones] [🌈][url-colores] [☑️][url-tablas] [📺][url-videos]  [🔣][url-ascii] [➗][url-matematicas]


Hecho con el 💚 en el 2K20. 

[⚫][url-repositorio]



[url-repositorio]: https://github.com/mistersoftware/Crea-aportes-geniales-en-Platzi-con-Markdown/blob/master/formatos-de-texto-citas-enlaces-y-codigo-para-mejorar-tus-aportes-con-markdown.md "Código fuente de esta publicación en GitHub"

[url-dillinger]: https://dillinger.io/ "Editor en línea de Markdown"
[url-stackedit]: https://stackedit.io/app#/ "Editor en línea de Markdown"
[url-imgur]: https://imgur.com/ "Servicio gratuito de imágenes de Reddit"
[url-recordit]: https://recordit.co/ "Graba tu pantalla"
[url-asciinema]: https://itsfoss.com/asciinema-record-terminal/ "Copia el texto desde el video a la terminal"
[url-codecogs]: https://www.codecogs.com/latex/eqneditor.php "Convierte código latex a imágenes"
[url-rmarkdown]: https://rmarkdown.rstudio.com/ "una versión extendida de Markdown"
[url-traduccion-hipotesis]: https://platzi.com/tutoriales/1319-discretas/6238-hipotesis-de-riemann-traduccion-al-espanol/ "Traducción Hipótesis"
[url-overleaf]: https://www.overleaf.com/ "Código laTex en la nube"
[url-medium]: https://medium.com/@luiscarlos_40534/sobre-la-cantidad-de-n%C3%BAmeros-primos-por-debajo-de-una-cantidad-dada-%C3%BCber-die-anzahl-der-799ff571dd9 "Traducccion de la hipotesis en Medium"
[url-mistersoftware]: https://github.com/mistersoftware "Sigueme en GitHub"
[url-luisca]: https://platzi.com/@luisca "Perfil en Platzi"


[url-img-servidores]: https://i.imgur.com/xsquSxI.gif "Servidores A B C"
[url-img-casco]: https://i.imgur.com/b1kbwbR.gif "Casco"
[url-img-subir-imagen]: https://i.imgur.com/XXBeF2X.gif "Como subir imágenes en Platzi"
[url-img-learning]: https://static.platzi.com/media/learningpath/banners/1c4f4add-87b9-44cc-ba30-4a8a134bf76e.jpg "Learning path"
[url-img-ecuacion]: https://i.imgur.com/P4PL4vb.gif "Ecuacion en laTex"
[url-img-codecogs]: https://i.imgur.com/t1bOxue.png "codecogs"
[url-img-escritura]: https://i.imgur.com/3gtTnRU.gif "animación pluma"
[url-img-vistoporjuan]: https://i.imgur.com/W0D6elt.gif "Subir imagen en Platzi"
[url-img-badge-slack]: https://static.platzi.com/media/achievements/badges-comunicacion-slack-60710bd2-a4fd-49e6-86af-bb12ed8e7417.png "bade slack"
[url-img-badge-escritura]: https://static.platzi.com/media/achievements/badge-escritura-online-1-ad291a75-10e8-426e-841d-fe66e340ccb6.png "badge escritura"
[url-ejemplo-color]: https://via.placeholder.com/75x16/98ca3f/444?text=Color "Color"
[url-ejemplo-boton]: https://via.placeholder.com/75x16/444/fcfcfc?text=Botones "Botones"
[url-img-proceso-md]: https://i.imgur.com/naN0LfO.png "Proceso de renderizado en Markdown"
[url-img-ascii]: https://i.imgur.com/DNgcFgx.png "Logo Platzi en ascii"


[url-platzi]: https://platzi.com/cursos "Nunca pares de aprender"
[url-connect]: https://platzi.com/empleos/ "Platzi Connect"
[url-curso-git]: https://platzi.com/clases/git-github/ "Curso Profesional de Git y GitHub"
[url-curso-slack]: https://platzi.com/clases/slack/ "Curso de Comunicación Online con Slack"
[url-curso-escritura]: https://platzi.com/clases/escritura-online/ "Curso de Escritura Online"
[url-pulse-editor]: https://platzi.com/blog/presentamos-pulse-editor/ "El sabor personalizado de Markdown en Platzi"

[url-indice]: https://platzi.com/blog/escribe-textos-geniales-con-markdown "✍️💡 Escribe textos geniales con Markdown 👨‍🎨👩‍🎨"
[url-textos]: https://platzi.com/comunidad/formatos-de-texto-citas-enlaces-y-codigo-para-mejorar-tus-aportes-con-markdown/ "✍️📖 Formatos de texto, citas, enlaces y código para mejorar tus aportes con Markdown 👨‍🎨👩‍🎨"
[url-imagenes]: https://platzi.com/comunidad/integrar-imagenes-en-tus-comentarios-o-tutoriales-con-markdown/ "✍️📷 Integrar imágenes en tus comentarios o tutoriales con Markdown 👨‍🎨👩‍🎨"
[url-animaciones]: https://platzi.com/comunidad/dale-vida-y-movimiento-a-tus-aportes-con-animaciones-con-markdown/ "✍️🎬 Dale vida y movimiento a tus aportes con animaciones con Markdown 👨‍🎨👩‍🎨"
[url-emojis]: https://platzi.com/comunidad/expresate-con-emojis-con-markdown/ "✍️🍕 Exprésate con Emojis con Markdown 👨‍🎨👩‍🎨"
[url-variables]: https://platzi.com/comunidad/agiliza-tu-escritura-con-variables-don-t-repeat-yourself-con-markdown/ "✍️🆎 Agiliza tu escritura con variables Don´t repeat yourself con Markdown 👨‍🎨👩‍🎨"
[url-botones]: https://platzi.com/comunidad/inserta-botones-para-facilitar-la-navegación-de-tus-lectores-con-markdown/ "✍️🔲 Inserta botones para facilitar la navegación de tus lectores con Markdown 👨‍🎨👩‍🎨"
[url-colores]: https://platzi.com/comunidad/color-y-alegria-en-tus-aportes-con-markdown/ "✍️🌈 Color y alegría en tus aportes con Markdown 👨‍🎨👩‍🎨"
[url-tablas]: https://platzi.com/comunidad/tablas-y-listas-tan-facil-como-nunca-lo-has-visto-con-markdown/ "✍️☑️ Tablas y listas tan fácil como nunca lo has visto con Markdown 👨‍🎨👩‍🎨"
[url-videos]: https://platzi.com/comunidad/incrusta-videos-en-tus-aportes-para-platzi-y-un-tip-para-incluirlos-en-github-con-markdown/ "✍️📺 Incrusta videos en tus aportes en Platzi y un tip para incluirlos en GitHub con Markdown 👨‍🎨👩‍🎨"
[url-ascii]: https://platzi.com/comunidad/ascii-art-branding-en-tu-codigo-con-markdown/ "✍️🔣 ASCII Art: branding en tu código con Markdown 👨‍🎨👩‍🎨"
[url-matematicas]: https://platzi.com/comunidad/bonus-inserta-formulas-matematicas-creadas-en-latex-con-markdown/ "✍️➗ Bonus: Inserta fórmulas matemáticas creadas en laTex con Markdown 👨‍🎨👩‍🎨"
[url-emojis-todos]: https://platzi.com/comunidad/listado-completo-de-emojis-en-markdown/ "✍️😍 Listado completo de emojis en Markdown 👨‍🎨👩‍🎨"


