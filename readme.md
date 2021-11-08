# TAREA EJERCICIOS JSX

## PARTICIPANTES
1. Santiago Gomez Garcia
##

### EJERCICIO 1

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 1.

        const data = {
            title_1: "Plato de la semana",
            title_2: "Berenjenas fritas",
            paragraph_1: "Comensales: 4 personas",
            paragraph_2: "Tiempo de reparación: 10 minutos",
            paragraph_3: "Tiempo de cocción: 12 minutos",
            paragraph_4: "Ingredientes:",
            paragraph_5: "4 berenjenas",
            paragraph_6: "Sal",
            paragraph_7: "Pimienta",
            paragraph_8: "4 cucharadas de harina y aceite",
            paragraph_9: "Preparación:",
            paragraph_10: "Lavar las berenjenas",
            paragraph_11: "Cortarlas en rodajas",
            paragraph_12: "Espolvorearlas con sal",
            paragraph_13: "Dejar que suelten el agua durante 30 minutos",
            paragraph_14: "Enharizarlas, ponerlas a freir durante 5 minutos en aceite bien caliente",
        }

        const title_x = <h1>{data.title_1}</h1>;
        const subtitle_x = <h2>{data.title_2}</h2>;
        const paragraph_x = <p>{data.paragraph_1}</p>;
        const paragraph_2x = <p>{data.paragraph_2}</p>;
        const paragraph_3x = <p>{data.paragraph_3}</p>;
        const paragraph_4x = <p>{data.paragraph_4}</p>;
        const paragraph_5x = <p>{data.paragraph_5}</p>;
        const paragraph_6x = <p>{data.paragraph_6}</p>;
        const paragraph_7x = <p>{data.paragraph_7}</p>;
        const paragraph_8x = <p>{data.paragraph_8}</p>;
        const paragraph_9x = <p>{data.paragraph_9}</p>;
        const paragraph_10x = <p>{data.paragraph_10}</p>;
        const paragraph_11x = <p>{data.paragraph_11}</p>;
        const paragraph_12x = <p>{data.paragraph_12}</p>;
        const paragraph_13x = <p>{data.paragraph_13}</p>;
        const paragraph_14x = <p>{data.paragraph_14}</p>;

        const element = (
            <div>
                {title_x}
                {subtitle_x}
                {paragraph_x}
                {paragraph_2x}
                {paragraph_3x}
                <br></br>
                {paragraph_4x}
                <ul>
                    <li>{paragraph_5x}</li>
                    <li>{paragraph_6x}</li>
                    <li>{paragraph_7x}</li>
                    <li>{paragraph_8x}</li>
                </ul>
                <br></br>
                {paragraph_9x}
                <ol>
                    <li>{paragraph_10x}</li>
                    <li>{paragraph_11x}</li>
                    <li>{paragraph_12x}</li>
                    <li>{paragraph_13x}</li>
                    <li>{paragraph_14x}</li>
                </ol>
            </div>
        );
        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 2

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 2.

        const data = {
            title_1: "Página inicial de Juan Tuesta",
            title_2: "Enlaces favoritos:",
            paragraph_1: "Bienvenido a mi página personal. Soy un alumno de la Universidad de Deusto y esta es mi página inicial, con la lista de mis enlaces favoritos y otra información de interés",
            paragraph_2: "Internet",
            paragraph_3: "Google",
            paragraph_4: "Aldea global",
            paragraph_5: "Manual de HTML",
            paragraph_6: "Juan Tuesta, Universidad de Deusto, marzo 2002.",
        }
        const titulo_x = <h1>{data.title_1}</h1>;
        const subtitulo_x = <h2>{data.title_2}</h2>;
        const parrafo_x = <p>{data.paragraph_1}</p>;
        const parrafo_2x = <p>{data.paragraph_2}</p>;
        const parrafo_3x = <p>{data.paragraph_3}</p>;
        const parrafo_4x = <p>{data.paragraph_4}</p>;
        const parrafo_5x = <p>{data.paragraph_5}</p>;
        const parrafo_6x = <p class="p1">{data.paragraph_6}</p>;

        const element = (
            <div>
                {titulo_x}
                {parrafo_x}
                {subtitulo_x}
                <ol>
                    <li>{parrafo_2x}</li>
                    <li>{parrafo_3x}</li>
                    <li>{parrafo_4x}</li>
                    <li>{parrafo_5x}</li>
                </ol>
                {parrafo_6x}
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 3

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 3.

        const data = {
            title_1: "Página inicial de Juan Tuesta",
            title_2: "Enlaces favoritos:",
            paragraph_1: "Bienvenido a mi página personal. Soy un alumno de la Universidad de Deusto y esta es mi página inicial, con la lista de mis enlaces favoritos y otra información de interés",
            paragraph_2: "Internet",
            paragraph_3: "Google",
            paragraph_4: "Aldea global",
            paragraph_5: "Manual de HTML",
            paragraph_6: "Juan Tuesta, Universidad de Deusto, marzo 2002.",
        }
        const titulox = <h1>{data.title_1}</h1>;
        const subtitulox = <h2>{data.title_2}</h2>;
        const parrafox = <p>{data.paragraph_1}</p>;
        const parrafo2x = <p>{data.paragraph_2}</p>;
        const parrafo3x = <p>{data.paragraph_3}</p>;
        const parrafo4x = <p>{data.paragraph_4}</p>;
        const parrafo5x = <p>{data.paragraph_5}</p>;
        const parrafo6x = <p class="p1">{data.paragraph_6}</p>;

        const element = (
            <div>
                {titulox}
                {parrafox}
                {subtitulox}
                <ol>
                    <li>{parrafo2x}</li>
                    <li><a href="tarea_jsx.html">{parrafo3x}</a></li>
                    <li>{parrafo4x}</li>
                    <li><a href="tarea_jsx.html">{parrafo5x}</a></li>
                </ol>
                {parrafo6x}
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 4

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 4.

        const data = {
            title_1: "Página inicial de Juan Tuesta",
            title_2: "Enlaces favoritos:",
            paragraph_1: "Bienvenido a mi página personal. Soy un alumno de la Universidad de Deusto y esta es mi página inicial, con la lista de mis enlaces favoritos y otra información de interés",
            paragraph_2: "Páginas personales",
            paragraph_3: "Páginas de referencia",
            paragraph_4: "Portales",
            paragraph_5: "Medios de comunicación",
            paragraph_6: "Charkes F.Golfarb",
            paragraph_7: "Lou Burnard",
            paragraph_8: "Tim Berners-Lee",
            paragraph_9: "Juan Tuesta, Universidad de Deusto, marzo 2002.",
        }
        const titulox1 = <h1>{data.title_1}</h1>;
        const subtitulox1 = <h2>{data.title_2}</h2>;
        const parrafox1 = <p>{data.paragraph_1}</p>;
        const parrafox2 = <p>{data.paragraph_2}</p>;
        const parrafox3 = <p>{data.paragraph_3}</p>;
        const parrafox4 = <p>{data.paragraph_4}</p>;
        const parrafox5 = <p>{data.paragraph_5}</p>;
        const parrafox6 = <p>{data.paragraph_6}</p>;
        const parrafox7 = <p>{data.paragraph_7}</p>;
        const parrafox8 = <p>{data.paragraph_8}</p>;
        const parrafox9 = <p class="p1">{data.paragraph_9}</p>;

        const element = (
            <div>
                {titulox1}
                {parrafox1}
                {subtitulox1}
                <ol>
                    <li>{parrafox2}</li>
                    <ul>
                        <li>{parrafox6}</li>
                        <li>{parrafox7}</li>
                        <li>{parrafox8}</li>
                    </ul>
                    <li>{parrafox3}</li>
                    <li>{parrafox4}</li>
                    <li>{parrafox5}</li>
                </ol>
                {parrafox9}
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 5

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 5.

        const data = {
            title_1: "Página inicial de Juan Tuesta",
            title_2: "Enlaces favoritos",
            title_3: "Páginas personales",
            title_4: "Páginas de referencia",
            title_5: "Portales",
            title_6: "Publicaciones",
            paragraph_1: "Bienvenido a mi página personal. Soy un alumno de la Universidad de Deusto y esta es mi página inicial, con la lista de mis enlaces favoritos y otra información de interés",
            paragraph_2: "Juan Tuesta, Universidad de Deusto, marzo 2002.",
            paragraph_3: "Páginas personales",
            paragraph_4: "Páginas de referencia",
            paragraph_5: "Portales",
            paragraph_6: "Publicaciones",
            paragraph_7: "Documentalistas",
            paragraph_8: "Historiadores",
            paragraph_9: "Lingüistas",
            paragraph_10: "Traductores",
            paragraph_11: "Bibliotecas universitarias",
            paragraph_12: "Centros de documentación",
            paragraph_13: "Museos de arte contemporáneo",
            paragraph_14: "Medios de comunicación",
            paragraph_15: "Inicia",
            paragraph_16: "Telépolis",
            paragraph_17: "Ciudades",
            paragraph_18: "Terra",
            paragraph_19: "Ciberp@ís",
            paragraph_20: "Diario Tecnologías de la Información",
            paragraph_21: "The Standard",
            paragraph_22: "Infoworld",
            paragraph_23: "Wired",
            paragraph_24: "Charkes F.Golfarb",
            paragraph_25: "Lou Burnard",
            paragraph_26: "Tim Berners-Lee",
        }
        const titulo1 = <h1>{data.title_1}</h1>;
        const subtitulo1 = <h2>{data.title_2}</h2>;
        const subtitulo2 = <h2>{data.title_3}</h2>;
        const subtitulo3 = <h2>{data.title_4}</h2>;
        const subtitulo4 = <h2>{data.title_5}</h2>;
        const subtitulo5 = <h2>{data.title_6}</h2>;
        const parrafo1 = <p>{data.paragraph_1}</p>;
        const parrafo2 = <p class="p1">{data.paragraph_2}</p>;
        const parrafo3 = <p>{data.paragraph_3}</p>;
        const parrafo4 = <p>{data.paragraph_4}</p>;
        const parrafo5 = <p>{data.paragraph_5}</p>;
        const parrafo6 = <p>{data.paragraph_6}</p>;
        const parrafo7 = <p>{data.paragraph_7}</p>;
        const parrafo8 = <p>{data.paragraph_8}</p>;
        const parrafo9 = <p>{data.paragraph_9}</p>;
        const parrafo10 = <p>{data.paragraph_10}</p>;
        const parrafo11 = <p>{data.paragraph_11}</p>;
        const parrafo12 = <p>{data.paragraph_12}</p>;
        const parrafo13 = <p>{data.paragraph_13}</p>;
        const parrafo14 = <p>{data.paragraph_14}</p>;
        const parrafo15 = <p>{data.paragraph_15}</p>;
        const parrafo16 = <p>{data.paragraph_16}</p>;
        const parrafo17 = <p>{data.paragraph_17}</p>;
        const parrafo18 = <p>{data.paragraph_18}</p>;
        const parrafo19 = <p>{data.paragraph_19}</p>;
        const parrafo20 = <p>{data.paragraph_20}</p>;
        const parrafo21 = <p>{data.paragraph_21}</p>;
        const parrafo22 = <p>{data.paragraph_22}</p>;
        const parrafo23 = <p>{data.paragraph_23}</p>;
        const parrafo24 = <p>{data.paragraph_24}</p>;
        const parrafo25 = <p>{data.paragraph_25}</p>;
        const parrafo26 = <p>{data.paragraph_26}</p>;

        const element = (
            <div>
                {titulo1}
                {parrafo1}
                {subtitulo1}
                <ol>
                    <li><a href="ejercicio5.html">{parrafo3}</a></li>
                    <li>{parrafo4}</li>
                    <li>{parrafo5}</li>
                    <li>{parrafo6}</li>
                </ol>
                <hr></hr>

                {subtitulo2}
                <ol>
                    <li>{parrafo7}</li>
                    <ul>
                        <li>{parrafo24}</li>
                        <li>{parrafo25}</li>
                        <li>{parrafo26}</li>
                    </ul>
                    <li>{parrafo8}</li>
                    <li>{parrafo9}</li>
                    <li>{parrafo10}</li>
                </ol>
                <hr></hr>

                {subtitulo3}
                <ol>
                    <li>{parrafo11}</li>
                    <li>{parrafo12}</li>
                    <li>{parrafo13}</li>
                    <li>{parrafo14}</li>
                </ol>
                <hr></hr>

                {subtitulo4}
                <ol>
                    <li>{parrafo15}</li>
                    <li>{parrafo16}</li>
                    <li>{parrafo17}</li>
                    <li>{parrafo18}</li>
                </ol>
                <hr></hr>

                {subtitulo5}
                <ol>
                    <li>{parrafo19}</li>
                    <li>{parrafo20}</li>
                    <li>{parrafo21}</li>
                    <li>{parrafo22}</li>
                    <li>{parrafo23}</li>
                </ol>
                <hr></hr>

                {parrafo2}

            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 6

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 6.

        const data = {
            title_1: "Next University",
            title_2: "Programas de Tecnología",
            title_3: "Desarrollador Web",
            title_4: "Android",
            title_5: "Programa de Negocio",
            title_6: "Mercadeo Digital",

        }

        const element = (
            <div>
                <h1>El Noticiero {data.title_1}</h1>
                <h2>{data.title_2}</h2>
                <h3>{data.title_3}</h3>
                <p><b>{data.title_1}</b> lanza su programa de formación <b>"{data.title_3}"</b> con la facilidad de cpacitar a personas en las tendencias actuales
                    sobre tecnologias, en caso de desarrollo web, se basa temas relacionados con implementacion de Front-End con tecnologias y Frameworks, tales
                    como: <i>HTML, CSS, JavaScript, Bootstrap, entre otros.</i></p>
                <h3>{data.title_4}</h3>
                <p>En <b>{data.line_1}</b> te ofrecemos el programa <b>{data.title_4}</b> que te da las herramientas necesarias para diseñar e implementar
                    aplicaciones {data.title_4} para dispositivos móviles, partiendo de un conocimiento basico de <i>Java</i>, utilizando el entorno de desarrollo de
                    <i>{data.title_4} Studio</i>. Aprenderás los aspectos fundamentales para crear aplicaiones {data.title_4} interactivas, dinámicas y exitosas
                    utilizando técnicas para el manejo de los recursos, datros, segundos planos, localizacion, sensores, animaciones, gráficos, multimedia y monetización.</p>
                <h2>{data.title_5}</h2>
                <h3>{data.title_6}</h3>
                <p><b><i>{data.title_1}</i></b> coloca a tu disposición el programa de <b>"{data.title_6}"</b>. Sabias que...{data.title_6} o Digital Marketing
                    es mucho mas que hacer y publicar anuncios. Se trata del consumidor y la estrategia de negocio.
                    Estos son los puntos de partida para que cualquier acción de {data.title_6} <i>sea exitosa y optimice la inversión.</i>
                    Este certificado, es un programa completo y práctico que permite entender al consumidor, la industria, la competencia y los retos del negocio propio;
                    para crear e implementar estrategias a la medida, en diferentes plataformas y medios digitales. Por supuesto, monitoreando los resultados para tomar
                    decisiones en tiempo real.</p>
            </div>
        );


        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 7

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 7.
        const data = {
            title_1: "Destinos Turísticos", title_2: "América",
            paragraph_1: "Argentina", paragraph_2: "Brasil", paragraph_3: "Chile",
            paragraph_4: "Colombia", paragraph_5: "Estados Unidos", paragraph_6: "México",
            paragraph_7: "Perú", paragraph_8: "Venezuela", paragraph_9: "Buenos Aires",
            paragraph_10: "Bariloche", paragraph_11: "Río de Janeiro", paragraph_12: "Brasilia",
            paragraph_13: "Santiago", paragraph_14: "Valparaiso", paragraph_15: "Bogotá",
            paragraph_16: "Cartagena de Indias", paragraph_17: "New York", paragraph_18: "San Francisco",
            paragraph_19: "Cancún", paragraph_20: "Acapulco", paragraph_21: "Lima",
            paragraph_22: "Cuzco", paragraph_23: "Margarita", paragraph_24: "Mérida",
        }
        const titular1 = <h1>{data.title_1}</h1>;
        const subtitular = <h2>{data.title_2}</h2>;
        const parrafito = <p>{data.paragraph_1}</p>;
        const parrafito2 = <p>{data.paragraph_2}</p>;
        const parrafito3 = <p>{data.paragraph_3}</p>;
        const parrafito4 = <p>{data.paragraph_4}</p>;
        const parrafito5 = <p>{data.paragraph_5}</p>;
        const parrafito6 = <p>{data.paragraph_6}</p>;
        const parrafito7 = <p>{data.paragraph_7}</p>;
        const parrafito8 = <p>{data.paragraph_8}</p>;
        const parrafito9 = <p>{data.paragraph_9}</p>;
        const parrafito10 = <p>{data.paragraph_10}</p>;
        const parrafito11 = <p>{data.paragraph_11}</p>;
        const parrafito12 = <p>{data.paragraph_12}</p>;
        const parrafito13 = <p>{data.paragraph_13}</p>;
        const parrafito14 = <p>{data.paragraph_14}</p>;
        const parrafito15 = <p>{data.paragraph_15}</p>;
        const parrafito16 = <p>{data.paragraph_16}</p>;
        const parrafito17 = <p>{data.paragraph_17}</p>;
        const parrafito18 = <p>{data.paragraph_18}</p>;
        const parrafito19 = <p>{data.paragraph_19}</p>;
        const parrafito20 = <p>{data.paragraph_20}</p>;
        const parrafito21 = <p>{data.paragraph_21}</p>;
        const parrafito22 = <p>{data.paragraph_22}</p>;
        const parrafito23 = <p>{data.paragraph_23}</p>;
        const parrafito24 = <p>{data.paragraph_24}</p>;

        const element = (
            <div class="contenido">
                {titular1}
                {subtitular}
                <ol class="contenido">
                    <li>{parrafito}</li>
                    <ol class="a">
                        <li>{parrafito9}</li>
                        <li>{parrafito10}</li>
                    </ol>
                    <li>{parrafito2}</li>
                    <ol class="b">
                        <li>{parrafito11}</li>
                        <li>{parrafito12}</li>
                    </ol>
                    <li>{parrafito3}</li>
                    <ol class="c">
                        <li>{parrafito13}</li>
                        <li>{parrafito14}</li>
                    </ol>
                    <li>{parrafito4}</li>
                    <ol class="d">
                        <li>{parrafito15}</li>
                        <li>{parrafito16}</li>
                    </ol>
                    <li>{parrafito5}</li>
                    <ol class="e">
                        <li>{parrafito17}</li>
                        <li>{parrafito18}</li>
                    </ol>
                    <li>{parrafito6}</li>
                    <ol class="f">
                        <li>{parrafito19}</li>
                        <li>{parrafito20}</li>
                    </ol>
                    <li>{parrafito7}</li>
                    <ol class="g">
                        <li>{parrafito21}</li>
                        <li>{parrafito22}</li>
                    </ol>
                    <li>{parrafito8}</li>
                    <ol class="h">
                        <li>{parrafito23}</li>
                        <li>{parrafito24}</li>
                    </ol>
                </ol>
            </div>
        );


        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 8

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 8.

        const data = {
            titulo: "Tu concierto",
            parrafo: "Bienvenido a este blog de conciertos",
        }

        const titulito = <h1 class="title">{data.titulo}</h1>;
        const parrafato = <p>{data.parrafo}</p>;


        const element = (
            <div>
                <img src="./multimedia/silueta-de-personas-celebrando.jpg" width="150" align="left" />
                {titulito}
                <br /><br /><br />
                {parrafato}
                <img src="./multimedia/los-oidos-concierto.jpg" />
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 9

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 9.

        const data = {
            title_1: "Cartelera de vuelos - Aeropuerto el mirador",
            title_2: "Llegadas",
            title_3: "Salidas",
            paragraph_1: "Aerolinea",
            paragraph_2: "Nro. vuelo",
            paragraph_3: "Estatus",
            paragraph_4: "Hora estimada",
            paragraph_5: "Puerta",
            paragraph_6: "AIRLAN",
            paragraph_7: "355",
            paragraph_8: "Aterrizo",
            paragraph_9: "Embarcando",
            paragraph_10: "3",
            paragraph_11: "1",
            paragraph_12: "2:45pm",
            paragraph_13: "2:15pm",

        }
        const tituloavion = <h1>{data.title_1}</h1>;
        const subtituloavion1 = <h2>{data.title_2}</h2>;
        const subtituloavion2 = <h2>{data.title_3}</h2>;
        const parrafoavion = <p>{data.paragraph_1}</p>;
        const parrafoavion2 = <p>{data.paragraph_2}</p>;
        const parrafoavion3 = <p>{data.paragraph_3}</p>;
        const parrafoavion4 = <p>{data.paragraph_4}</p>;
        const parrafoavion5 = <p>{data.paragraph_5}</p>;
        const parrafoavion6 = <p>{data.paragraph_6}</p>;
        const parrafoavion7 = <p>{data.paragraph_7}</p>;
        const parrafoavion8 = <p>{data.paragraph_8}</p>;
        const parrafoavion9 = <p>{data.paragraph_9}</p>;
        const parrafoavion10 = <p>{data.paragraph_10}</p>;
        const parrafoavion11 = <p>{data.paragraph_11}</p>;
        const parrafoavion12 = <p>{data.paragraph_12}</p>;
        const parrafoavion13 = <p>{data.paragraph_13}</p>;


        const element = (
            <div>
                {tituloavion}
                {subtituloavion1}
                <table border="1">
                    <thead>
                        <tr>
                            <th>{parrafoavion}</th>
                            <th>{parrafoavion2}</th>
                            <th>{parrafoavion3}</th>
                            <th>{parrafoavion4}</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>{parrafoavion6}</td>
                            <td>{parrafoavion7}</td>
                            <td>{parrafoavion8}</td>
                            <td>{parrafoavion12}</td>
                        </tr>
                    </tbody>
                </table>
                {subtituloavion2}
                <table border="1">
                    <thead>
                        <tr>
                            <th>{parrafoavion}</th>
                            <th>{parrafoavion2}</th>
                            <th>{parrafoavion3}</th>
                            <th>{parrafoavion4}</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>{parrafoavion6}</td>
                            <td>{parrafoavion7}</td>
                            <td>{parrafoavion9}</td>
                            <td>{parrafoavion13}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 10

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 10.

        const datos = {

            titulo1: "Recetas.com",
            img: "./multimedia/cartoonchef.jpg",
            menu1: "Recetas Principales   ",
            barra: "|",
            menu2: " Postres latinos",
            parrafo1: "Bienvenidos a nuestro sitio Web sobre gastronomia latina, te invitamos a preparar nuestras recetas",
            titulo2: "Nuevas Recetas",
            parrafo2: "**Arroz Criollo*",
            parrafo3: "Tiempo de preparación: ",
            parrafo4: "45 minutos",
            parrafo5: "Numero de porciones",
            parrafo6: "4",
            parrafo7: "Ingredientes",
            v1: "Salsa de tomate",
            v2: "2 cucharadas de aceite 14gr",
            v3: "1 cebolla larga picada 45gr",
            v4: "2 dientes de ajo finamente picado 3gr",
            v5: "1 pimentón rojo picado en cuadritos 60gr",
            v6: "1 taza de arroz blanco 225gr",
            v7: "1 taza de maíz desgranado 79gr",
            v8: "150gr de pechuga de pollo cocinado y desmechado",
            v9: "Sal al gusto",
            parrafo8: "Preparación",
            v10: "Calentar en una olla el aceite, sofreir la cebolla junto con el ajo, el pimentin por 3 minutos",
            v11: "Adicionar el arroz y continua sofriendo para que se dore.",
            v12: "Agregar el pollo, el maiz desgranado y las verduras.",
            v13: "Mezclar todo, rectificar sal y dejar cocinar hasta que seque.",
            v14: "Bajar el fuego, tapar la olla y continuar la cocción por 25 minutos más.",
            parrafo9: "Esta rica receta fue proporcionada por Maria Paula.",
        }

        const element = (
            <div>
                <h1> {<img src={datos.img} width="150" />} {datos.titulo1}</h1>
                <h3><a href="">{datos.menu1}</a>  {datos.barra}  <a href=""> {datos.menu2}</a></h3>
                <br />
                <p>{datos.parrafo1}</p>
                <h1>{datos.titulo2}</h1>
                <h2>{datos.parrafo2}</h2>
                <p>{datos.parrafo3} <b>{datos.parrafo4}</b> {datos.parrafo5} <b>{datos.parrafo6}</b> </p>
                <h2>{datos.parrafo7}</h2>
                <ul>
                    <li><b>{datos.v1}</b></li>
                    <br></br>
                    <li><b>{datos.v2}</b></li>
                    <br></br>
                    <li><b>{datos.v3}</b></li>
                    <br></br>
                    <li><b>{datos.v4}</b></li>
                    <br></br>
                    <li><b>{datos.v5}</b></li>
                    <br></br>
                    <li><b>{datos.v6}</b></li>
                    <br></br>
                    <li><b>{datos.v7}</b></li>
                    <br></br>
                    <li><b>{datos.v8}</b></li>
                    <br></br>
                    <li><b>{datos.v9}</b></li>
                </ul>
                <h2>{datos.parrafo8}</h2>
                <ol>
                    <li>{datos.v10}</li>
                    <br></br>
                    <li>{datos.v11}</li>
                    <br></br>
                    <li>{datos.v12}</li>
                    <br></br>
                    <li>{datos.v13}</li>
                    <br></br>
                    <li>{datos.v14}</li>
                </ol>
                <p>{datos.parrafo9}</p>
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 11

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 11.
        const data = {

            titulo1: "Registro en nuestra tienda",
            nombre: "Nombre de usuario:",
            email: "Email:",
            edad: "Edad:",
            genero: "Género:",
            recomendado: "Recomendado por:",
            comentarios: "Comentarios:",
            acepto: "Acepto terminos y condiciones:"

        }

        const element = (
            <div>
                <h1>{data.titulo1}</h1>
                <p>{data.nombre}</p>
                <input type="text" placeholder="Ej: luis" ></input>
                <br />
                <p>{data.email}</p>
                <input type="text" placeholder="Ej: luis@gmail.com" ></input>
                <br />
                <p>{data.edad}</p>
                <input type="text" placeholder="Ej: 21" ></input>
                <br />
                <p>{data.genero}</p>
                <input type="radio" value="Masculino" name="Genero" /> Masculino
                <br />
                <input type="radio" value="Femenino" name="Genero" /> Femenino
                <br />
                <p>{data.recomendado}</p>
                <select value={data.recomendado}>
                    <option value="A">Google</option>
                    <option value="B">Amazon</option>
                    <option value="C">Facebook</option>
                </select>
                <br />
                <p>{data.comentarios}</p>
                <textarea rows={4} cols={50} type="textarea"
                    name="textValue"
                />
                <br />
                <p>{data.acepto}</p>
                <input type="checkbox" />
                <br />
                <input type="submit" value="Registrar" />
            </div>
        );


        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 12

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 12.

        const data = {

            titulo: "Título en encabezado",
            descrip: "Descripción del audio",
            audio: "./multimedia/bensound-clearday.mp3",
            drechos: "Derechos Reservados (Pie)",

        }

        const element = (
            <div>
                <h1>{data.titulo}</h1>
                <p>{data.descrip}</p>
                <br />
                <audio controlsList="nodownload" controls>
                    <source src={data.audio} type="audio/mpeg" />
                </audio>
                <br />
                <br />
                <p>{data.drechos}</p>
            </div>
        );

        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```

### EJERCICIO 13

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <meta name="author" content="Santiago Gomez Garcia">
    <meta name="keywords" content="html, css, example, homework, basics, jsx">
    <meta name="description" content="Ejercicios JSX">
    <title></title>
    <link rel="stylesheet" type="text/css" media="screen" href="style.css" />
</head>

<body>
    <div id="root">
        <!--Render code React-js-->
    </div>

    <!-- Cargar React. -->
    <!-- Nota: cuando se despliegue, reemplazar "development.js" con "production.min.js". -->
    <script src="https://unpkg.com/react@16/umd/react.development.js"></script>
    <script src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <!-- Cargamos nuestro componente de React. -->
    <script type="text/babel">
        // nota cada codigo que veas documentado de aca para abajo
        // seran diferentes formas de realizarlo con jsx los coloco para
        // que podamos probar y mirar diferentes formas de como podriamos realizarlos
        // los 12 ejercicios

        // Ejercicio 13.

        const data = {

            titulo: "Título en encabezado",
            descrip: "Este es un párrafo",
            video: "./multimedia/New video.mp4",
            drechos: "Derechos Reservados (Pie)",

        }

        const element = (
            <div>
                <h1>{data.titulo}</h1>
                <p>{data.descrip}</p>
                <video width="750" height="500" controls >
                    <source src={data.video} type="video/mp4" />
                </video>
                <br />
                <br />
                <p>{data.drechos}</p>
            </div>
        );


        // Renderiamos o pintamos
        ReactDOM.render(
            element,// estructura jsx para pintar
            document.getElementById('root')// elemento donde se pintara
        );
    </script>
</body>

</html>
```