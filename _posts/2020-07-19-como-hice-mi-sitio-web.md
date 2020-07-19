---
title: 'Como he creado mi sitio web'
date: 2020-07-19 00:00:00
description: Te cuento como he creado este blog paso a paso.
featured_image: '/images/posts/01/israel-alcazar-ingeniero-humanista-web.png'
---

![](/images/posts/01/israel-alcazar-ingeniero-humanista-web.png)




Quiero dedicar el primer artículo de esta nueva etapa, explicando como he creado mi sitio web personal por si alguien mas pudiera estar interesado ya que he utilizado tecnologías alternativas al típico wordpress.

> “La simplicidad o el arte de maximizar la cantidad de trabajo no realizado resultan fundamental.”

## El propósito

Como no podría ser de otro modo, todo proyecto siempre debe comenzar pensando en el propósito o dicho de otro modo: ¿Para qué vas a hacerlo?. En mi caso era bastante sencillo. Con el paso de los años he ido generando una imagen profesional que se encuentra dispersa por la red. Mi principal objetivo con mi página personal es que fuera un *punto principal donde encontrar toda la información relacionada con mi persona*. Así de esta manera los diferentes artículos, videos o información relacionada con mi persona serán sencillos de acceder. 

También quería tener todas mis redes y proyectos en los que pongo energía recopilados en un solo sitio para que todas las personas que quieran conocer mas acerca de mi puedan hacerlo de manera sencilla. No es que me haya vuelto loco y me crea un tipo interesante, al contrario, no espero que esta web tenga demasiadas visitas. Es algo mas para mi que espero también quede como recordatorio con el paso de los años. Debe ser la crisis de los 40.

Ya he intentado numerosas veces generar un sitio personal donde escribir. Nunca me ha terminado de funcionar ya que siempre lo orientaba a temas profesionales. En este caso, quiero cambiar el enfoque ya que todos los temas relacionados con lo profesional quiero que sigan estando en el *proyecto de vida* [Thinking With You](thinkingwithyou.com). Esta web, por el contrario, contendrá solo aquellos artículos que por circunstancias no tiene sentido publicar en Thinking. Bien porque sean personales e íntimos, bien porque la temática no tenga relación. Tengo diferentes algunos hobbies como la tecnología o viajar sobre los que me gustaría publicar. 

## Tecnología que utilizo

Una vez aclarado el pará que lo siguiente que me planteé era el "cómo". En otras ocasiones había optado por reservar un dominio con mi nombre e instalar un wordpress por su sencillez de manejo y la multido de plugins y posibilidades "para tontos" que contiene. Pero esta vez pensé en hacer algo mas sencillo todavía. Wordpress necesita un trabajo inicial importante y un posterior trabajo de mantenimiento y actualización progresiva, además de un especial cuidado con la seguridad al ser unas de las tecnologías mas utilizadas también es una de las más explotadas por hackers. Como lo que quería tampoco tiene demasiado complicación pensé en una solución que hace años ya probé para otros proyectos: [Github Pages](https://pages.github.com/) + [Jekyll](https://jekyllrb.com/) . 




Sigue leyendo que te cuento todo.

### Reservar el dominio

Lo primero que debes hacer si quieres tener tu web bajo un dominio propio (israelalcazar.com como en mi caso) es reservarlo. En mi caso he pasado por diferentes proveedores de dominios y cada cual tiene sus cosas buenas y malas. En este caso solo vamos a necesitar reservar el dominio ya que el alojamiento o hosting lo tendremos por otro lado. He probado en [Cdmon](cdmon.com), [godaddy](godaddy.com) o [Dreamhost](https://www.dreamhost.com/). En este último es donde actualmente tengo reservado mi dominio simplemente porque es el que utilizamos en Thinking With You y ya me conozco su administración. 

El precio del dominio puede variar entre los 5 o 15 € / año (si, has leído bien al año) en función de si quieres contratar un .com, .es, .org o cualquier otro. Actualmente existen multitud de tipos de dominios. También variará el precio en función del tiempo durante el cual lo contrates. No es lo mismo contratarlo por 3-6-12 meses o incluso por años. Mi recomendación es que lo contrates al menos por un año ya que te saldrá mas barato.

Si fueras a montar tu sitio web en Wordpress probablemente necesitarás tanto dominio como alojamiento donde montar la web. En mi caso utilizaré [Github Pages](https://pages.github.com/) como alojamiento. 

### Github Pages

Github Pages es una tecnología propuesta por Github para poder albergar de manera sencilla páginas web estáticas (esto es que solo tienen html, css y JavaScript). No posee la capacidad de tener base de datos o cualquier otra tecnología instalada. 

Y ¿por qué utilizaste esto? ¿Eres un poco friki no?. Si bueno, Ingerieron Humanista, así que mi parte ingenieril y de pasión por la tecnología me puede a veces y por eso me encanta probar cosas nuevas y experimentar.

Lo bueno de Github Pages es que cuenta con un motor que permite algo mas que solo tener páginas web estáticas. Permite algo de dinamismo gracias a Jekyll con el que he podido montar toda la infraestructura necesaria para generar las páginas y el blog. 


### Jekyll

Es una tecnología en Ruby que permite generar sitios web estáticos de una manera muy simple. Aquí te dejo una primera página donde cuenta como empezar con los [primeros pasos](https://jekyllrb.com/docs/usage/). 

**NOTA: Es necesario cierto conocimiento tecnológico para trabajar con Jekyll así que si no cuentas con unos mínimos conocimientos de Ruby, desarrollo web y programación básica te recomiendo que no vayas a esta solución y que lo mejor será un [Wordpress](wordpress.org).**

### Jekyll Themes

Para evitarme tener que partir de cero a la hora de realizar mi sitio web (estoy mayor ya para esto) me he basado en un tema de [los muchos](https://jekyll-themes.com/) con los que cuenta Jekyll para contar con toda la estructura necesaria. En mi caso he elegido Duet por la recomendación de [Leonardo Poza](http://leonardopoza.com/) (gracias Leo).


## Cómo hice esta web

Bien, pues una vez que os he contado la tecnología que utilizo. Ahora te cuento como. 

**1.Lo primero es reservar el dominio.**
Ya te he comentado mas arriba que puedes utilizar diferentes empresas para poder hacerlo y que su coste varía en función del tipo de dominio y el tiempo contratado. Puede ser entre 5 o 15 € aproximadamente.

**2.Referencia al DNS desde tu dominio**
Una vez reservado el dominio debes hacer referencia en su DNS a los servidores de Github:

![](/images/posts/01/01-dns.png)

**3.Crear un repositorio en GitHub**
Para poder utilizar Github Pages debes generar un nuevo repositorio dentro de Github que se llame como <tu usuario>.github.io

![](/images/posts/01/02-settings.png)

**4.Configuración del dominio en GitHub**
Dentro de la configuración (settings) deberás indicar el nombre del dominio.

![](/images/posts/01/03-github-pages.png)

**5.Fichero CNAME dentro de tu repositorio**
Por último, dentro de tu repositorio debes tener un fichero CNAME con el nombre de tu dominio dentro (israelalcazar.com en mi caso)

Y listo. Parece muy difícil pero si sigues los pasos correctamente todo acaba funcionando.

**Bola Extra: Si quieres que tu sitio sea seguro deberás instalar un certificado en tu dominio y después marcar la casilla "ENFORCE HTTPS" dentro de la configuración de GitHub.**

Aquí te dejo un sencillo tutorial con los pasos mejor explicados:
[https://docs.github.com/en/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site](https://docs.github.com/en/github/working-with-github-pages/configuring-a-custom-domain-for-your-github-pages-site)