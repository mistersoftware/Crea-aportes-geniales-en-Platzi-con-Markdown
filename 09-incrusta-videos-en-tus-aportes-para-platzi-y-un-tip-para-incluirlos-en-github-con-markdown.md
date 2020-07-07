✍️📺 Incrusta videos en tus aportes en Platzi y un tip para incluirlos en GitHub con Markdown 👨‍🎨👩‍🎨


_Anterior:_ ⏪ [_Tablas y listas tan facil como nunca lo has visto_][url-tablas]  ☑️

==«==
---
 
 
> _**" Esta publicación forma parte de una serie denominada: 🇪🇸 ✍️💡 [ Escribe textos geniales con Markdown][url-indice] 👨‍🎨👩‍🎨. Si has llegado aquí sin pasar por allí, te recomiendo visitarla, donde encontraras el índice principal. "**_


==»==
---


## 📺 Incrustar videos 

## YouTube en Platzi 

Para incrustar o insertar videos, es decir, que se puedan reproducir allí mismo sin que el lector deba ir a otra página, deberemos utilizar la siguiente sintaxis:

==«==
---

`@[youtube](ZYmIUiK8ZQI|https://www.youtube.com/watch?v=ZYmIUiK8ZQI)`



==» El código anterior producirá:»==
---

  @[youtube](ZYmIUiK8ZQI|https://www.youtube.com/watch?v=ZYmIUiK8ZQI)


---





## Vimeo en Platzi 

==«==
---

`@[vimeo](427943407|https://vimeo.com/427943407/)`


==» El código anterior producirá: »==
---


@[vimeo](128154222|https://vimeo.com/128154222/)


## Insertar miniatura con enlace al video (Funciona en todas partes incluido GitHub)

Valga la aclaración que con este método **no es necesario descargar la thumbnail**, pues la etiqueta está escrita para que la tome automáticamente de la API de Youtube.


## Usando Youtube API

| Nombre de miniatura      | Tamaño (px) | URL                                              |
|---------------------|-----------|--------------------------------------------------|
| Player Background   | 480x360   | https://i1.ytimg.com/vi/«ID»/0.jpg         |
| Start               | 120x90    | https://i1.ytimg.com/vi/«ID»/1.jpg         |
| Middle              | 120x90    | https://i1.ytimg.com/vi/«ID»/2.jpg         |
| End                 | 120x90    | https://i1.ytimg.com/vi/«ID»/3.jpg         |
| High Quality        | 480x360   | https://i1.ytimg.com/vi/«ID»/hqdefault.jpg |
| Medium Quality      | 320x180   | https://i1.ytimg.com/vi/«ID»/mqdefault.jpg |
| Normal Quality      | 120x90    | https://i1.ytimg.com/vi/«ID»/default.jpg 


 
==«==
---

````[background]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/0.jpg "background"
[start]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/1.jpg "start"
[middle]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/2.jpg "middle"
[end]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/3.jpg "end"
[hqdefault]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/hqdefault.jpg "hqdefault"
[mqdefault]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/mqdefault.jpg "mqdefault"
[default]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/default.jpg "default"
[urlYoutube]: https://www.youtube.com/watch?v=ZYmIUiK8ZQI "Titulo del video"


[![x][start]][urlYoutube] [![x][middle]][urlYoutube] [![x][end]][urlYoutube] [![x][default]][urlYoutube] [![x][mqdefault]][urlYoutube] [![x][hqdefault]][urlYoutube] [![x][background]][urlYoutube]
````




==» El Código anterior producirá:==
---

[background]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/0.jpg "background"
[start]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/1.jpg "start"
[middle]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/2.jpg "middle"
[end]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/3.jpg "end"
[hqdefault]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/hqdefault.jpg "hqdefault"
[mqdefault]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/mqdefault.jpg "mqdefault"
[default]: https://i1.ytimg.com/vi/ZYmIUiK8ZQI/default.jpg "default"
[urlYoutube]: https://www.youtube.com/watch?v=ZYmIUiK8ZQI "Titulo del video"


[![x][start]][urlYoutube] [![x][middle]][urlYoutube] [![x][end]][urlYoutube] [![x][default]][urlYoutube] [![x][mqdefault]][urlYoutube] [![x][hqdefault]][urlYoutube] [![x][background]][urlYoutube]


## Usando Vimeo API

Lo primero que debemos observar es la ID publica 128154222 y con ella realizamos el llamado a la api para obtener los datos del video, puedes elegir el formato que gustes
 
* [http://vimeo.com/api/v2/video/128154222.json](http://vimeo.com/api/v2/video/128154222.json)
* [http://vimeo.com/api/v2/video/128154222.php](http://vimeo.com/api/v2/video/128154222.php)
* [http://vimeo.com/api/v2/video/128154222.xml](http://vimeo.com/api/v2/video/128154222.xml)
 
Para este ejemplo hemos realizado la llamada al archivo json, y luego de pasarlo por [jsonbeautifier](https://jsonbeautifier.org) obtenemos
---

>````
>[
>  {
>    "id": 128154222,
>    "title": "Lytro Test Video",
>    "description": "A sample video create from a single still photo snapped with the Lytro Illum. Read our full review of the Illum here: http://bit.ly/1EXnxU8  © >David Patiño",
>    "url": "https://vimeo.com/128154222",
>    "upload_date": "2015-05-18 11:22:34",
>    "thumbnail_small": "http://i.vimeocdn.com/video/519177743_100x75.jpg",
>    "thumbnail_medium": "http://i.vimeocdn.com/video/519177743_200x150.jpg",
>    "thumbnail_large": "http://i.vimeocdn.com/video/519177743_640.jpg",
>    "user_id": 5862464,
>    "user_name": "PDNOnline",
>    "user_url": "https://vimeo.com/user5862464",
>    "user_portrait_small": "http://i.vimeocdn.com/portrait/5664890_30x30",
>    "user_portrait_medium": "http://i.vimeocdn.com/portrait/5664890_75x75",
>    "user_portrait_large": "http://i.vimeocdn.com/portrait/5664890_100x100",
>    "user_portrait_huge": "http://i.vimeocdn.com/portrait/5664890_300x300",
>    "stats_number_of_likes": 3,
>    "stats_number_of_plays": 843,
>    "stats_number_of_comments": 0,
>    "duration": 10,
>    "width": 1056,
>    "height": 720,
>    "tags": "Lytro, photography, cameras, technology",
>    "embed_privacy": "anywhere"
>  }
>]
>````
>
> **En la respuesta obtenemos los datos del id interno 519177743 y nos ofrece 3 tamaños de miniatura. Es necesario que el video no sea privado**

==«==
---

````
[![][small]][urlVimeo]
[![][medium]][urlVimeo]
[![][large]][urlVimeo]

[small]: https://i.vimeocdn.com/video/519177743_100x75.jpg "Small 100x75"
[medium]: https://i.vimeocdn.com/video/519177743_200x150.jpg "Medium 200x150"
[large]: https://i.vimeocdn.com/video/519177743_640.jpg "Large 640"
[urlVimeo]: https://vimeo.com/128154222/ "Vimeo"
````


==» El Código anterior producirá:==
---

[![][small]][urlVimeo]
[![][medium]][urlVimeo]
[![][large]][urlVimeo]

[small]: https://i.vimeocdn.com/video/519177743_100x75.jpg "Small 100x75"
[medium]: https://i.vimeocdn.com/video/519177743_200x150.jpg "Medium 200x150"
[large]: https://i.vimeocdn.com/video/519177743_640.jpg "Large 640"
[urlVimeo]: https://vimeo.com/128154222/ "Vimeo"




==«==
---

**_Continúa tu aprendizaje con:_**

* ⏩ [_ASCII Art: branding en tu código_][url-ascii] 🔣

==»==
---

[📖][url-textos] [📷][url-imagenes] [🎬][url-animaciones] [🍕][url-emojis] [🆎][url-variables] [🔲][url-botones] [🌈][url-colores] [☑️][url-tablas] [📺][url-videos]  [🔣][url-ascii] [➗][url-matematicas]


Hecho con el 💚 en el 2K20. 

[⚫][url-repositorio]

[url-repositorio]: https://github.com/mistersoftware/Crea-aportes-geniales-en-Platzi-con-Markdown/blob/master/09-incrusta-videos-en-tus-aportes-para-platzi-y-un-tip-para-incluirlos-en-github-con-markdown.md "Código fuente de esta publicación en GitHub"



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

