#Pagina web 
Este apartado se lo dedicamos para la preevisualizacion de la pagina web que utilizaremos 

index.html 

```html
<!-- index.html -->
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Agenda 2030 - Desarrollo Sostenible</title>
  <link rel="stylesheet" href="./css/style.css">
  <link rel="icon" type="image/png" href="assets/favicon/favicon.png">
</head>
<body>
    <header>
        <h1>El Futuro es Verde</h1>
        <h2>Objetivos de Desarrollo Sostenible 2030</h2>
        <nav>
          <ul>
            <li><a href="index.html">Inicio</a></li>
            <li><a href="sostenibilidad.html">Sostenibilidad</a></li>
            <li><a href="proyecto.html">Sobre el Proyecto</a></li>
          </ul>
        </nav>

        <button onclick="toggleModoEco()" class="boton-eco">🌱 Modo Eco</button>
      </header>
  <main>
    <section class="intro">
        <h2>Unidos por un futuro sostenible</h2>
        <p>Descubre los 17 Objetivos de Desarrollo Sostenible y acompáñanos en el camino hacia un mundo más justo, equitativo y respetuoso con el planeta.</p>
    </section>

    <section class="ods">
        <h2>Objetivos de Desarrollo Sostenible</h2>
        <div class="cards-container">

          <label for="ods1">
            <input type="radio" name="ods" id="ods1" hidden>
            <details class="card">
              <summary>ODS 1: Fin de la pobreza</summary>
              <p>Erradicar la pobreza en todas sus formas y dimensiones es un requisito indispensable para el desarrollo sostenible. Este objetivo busca garantizar el acceso universal a recursos básicos como alimentación, vivienda, servicios sanitarios y educación, además de fomentar políticas de protección social y empleo digno.</p>
            </details>
          </label>

          <label for="ods2">
            <input type="radio" name="ods" id="ods2" hidden>
            <details class="card">
              <summary>ODS 2: Hambre cero</summary>
              <p>El hambre y la malnutrición siguen siendo barreras fundamentales para el desarrollo. Este objetivo busca lograr la seguridad alimentaria, mejorar la nutrición y promover la agricultura sostenible mediante el apoyo a pequeños productores y la resiliencia frente al cambio climático.</p>
            </details>
          </label>
 
          <label for="ods3">
            <input type="radio" name="ods" id="ods3" hidden>
            <details class="card">
              <summary>ODS 3: Salud y bienestar</summary>
              <p>Garantizar vidas saludables y promover el bienestar para todos es esencial para un futuro próspero. Este objetivo abarca desde la reducción de la mortalidad infantil y materna hasta la cobertura sanitaria universal, salud mental y preparación frente a pandemias.</p>
            </details>
          </label>

          <label for="ods4">
            <input type="radio" name="ods" id="ods4" hidden>
            <details class="card">
              <summary>ODS 4: Educación de calidad</summary>
              <p>Este objetivo busca asegurar una educación inclusiva y de calidad en todos los niveles, así como fomentar oportunidades de aprendizaje permanente. Incluye la mejora de la formación docente, la equidad de género en el acceso a la educación y el desarrollo de habilidades digitales.</p>
            </details>
          </label>

          <label for="ods5">
            <input type="radio" name="ods" id="ods5" hidden>
            <details class="card">
              <summary>ODS 5: Igualdad de género</summary>
              <p>Promueve la eliminación de todas las formas de discriminación y violencia contra mujeres y niñas. Incluye el acceso igualitario a oportunidades económicas, liderazgo político, salud sexual y reproductiva, y la erradicación del matrimonio infantil.</p>
            </details>
          </label>

          <label for="ods6">
            <input type="radio" name="ods" id="ods6" hidden>
            <details class="card">
              <summary>ODS 6: Agua limpia y saneamiento</summary>
              <p>Busca garantizar el acceso universal y equitativo al agua potable y el saneamiento. Incluye la mejora de la calidad del agua, la eficiencia en su uso, la protección de ecosistemas acuáticos y la cooperación internacional en la gestión hídrica.</p>
            </details>
          </label>

          <label for="ods7">
            <input type="radio" name="ods" id="ods7" hidden>
            <details class="card">
              <summary>ODS 7: Energía asequible y no contaminante</summary>
              <p>Fomenta el acceso universal a servicios energéticos modernos, fiables y sostenibles. Promueve el uso de energías renovables, la mejora de la eficiencia energética y la inversión en tecnologías limpias, fundamentales para mitigar el cambio climático.</p>
            </details>
          </label>

          <label for="ods8">
            <input type="radio" name="ods" id="ods8" hidden>
            <details class="card">
              <summary>ODS 8: Trabajo decente y crecimiento económico</summary>
              <p>Este objetivo busca fomentar un crecimiento económico sostenido, inclusivo y sostenible. Promueve el empleo pleno y productivo, los derechos laborales, la reducción del desempleo juvenil y la erradicación del trabajo forzoso e infantil.</p>
            </details>
          </label>

          <label for="ods9">
            <input type="radio" name="ods" id="ods9" hidden>
            <details class="card">
              <summary>ODS 9: Industria, innovación e infraestructura</summary>
              <p>Aboga por construir infraestructuras resilientes, fomentar la industrialización inclusiva y promover la innovación tecnológica. Busca cerrar la brecha digital y mejorar la sostenibilidad de la infraestructura energética y de transporte.</p>
            </details>
          </label>

          <label for="ods10">
            <input type="radio" name="ods" id="ods10" hidden>
            <details class="card">
              <summary>ODS 10: Reducción de las desigualdades</summary>
              <p>Busca reducir las desigualdades dentro de los países y entre ellos, mediante políticas fiscales y sociales inclusivas, la protección de los derechos de los migrantes y la promoción de la equidad económica y social.</p>
            </details>
          </label>

          <label for="ods11">
            <input type="radio" name="ods" id="ods11" hidden>
            <details class="card">
              <summary>ODS 11: Ciudades y comunidades sostenibles</summary>
              <p>Promueve ciudades inclusivas, seguras, resilientes y sostenibles. Abarca desde el acceso a viviendas adecuadas hasta el transporte sostenible, la gestión de residuos urbanos y la planificación urbana respetuosa con el medio ambiente.</p>
            </details>
          </label>

          <label for="ods12">
            <input type="radio" name="ods" id="ods12" hidden>
            <details class="card">
              <summary>ODS 12: Producción y consumo responsables</summary>
              <p>Busca garantizar patrones sostenibles de consumo y producción, fomentando la eficiencia de recursos, la gestión ecológica de productos químicos y desechos, y el acceso a información para adoptar decisiones responsables.</p>
            </details>
          </label>

          <label for="ods13">
            <input type="radio" name="ods" id="ods13" hidden>
            <details class="card">
              <summary>ODS 13: Acción por el clima</summary>
              <p>Insta a adoptar medidas urgentes para combatir el cambio climático y sus efectos. Esto incluye la mejora de la educación ambiental, la resiliencia frente a desastres naturales y el cumplimiento de acuerdos internacionales como el Acuerdo de París.</p>
            </details>
          </label>

          <label for="ods14">
            <input type="radio" name="ods" id="ods14" hidden>
            <details class="card">
              <summary>ODS 14: Vida submarina</summary>
              <p>Promueve la conservación y el uso sostenible de los océanos, mares y recursos marinos. Incluye la reducción de la contaminación marina, la protección de ecosistemas costeros y la pesca sostenible.</p>
            </details>
          </label>

          <label for="ods15">
            <input type="radio" name="ods" id="ods15" hidden>
            <details class="card">
              <summary>ODS 15: Vida de ecosistemas terrestres</summary>
              <p>Se centra en proteger, restaurar y promover el uso sostenible de los ecosistemas terrestres. Abarca la gestión de bosques, la lucha contra la desertificación y la pérdida de biodiversidad, vital para la salud del planeta.</p>
            </details>
          </label>

          <label for="ods16">
            <input type="radio" name="ods" id="ods16" hidden>
            <details class="card">
              <summary>ODS 16: Paz, justicia e instituciones sólidas</summary>
              <p>Busca promover sociedades justas, pacíficas e inclusivas. Esto incluye el acceso a la justicia, la lucha contra la corrupción, instituciones transparentes y la participación ciudadana.</p>
            </details>
          </label>

          <label for="ods17">
            <input type="radio" name="ods" id="ods17" hidden>
            <details class="card">
              <summary>ODS 17: Alianzas para lograr los objetivos</summary>
              <p>Este objetivo reconoce que la cooperación internacional es esencial para lograr el desarrollo sostenible. Fomenta alianzas globales inclusivas, la movilización de recursos financieros y la transferencia de tecnología.</p>
            </details>
          </label>
        </div>
      </section>
  </main>
  <footer>
    <p>Desarrollado en Raspberry Pi con energía solar. Proyecto para el módulo de Sostenibilidad en el Sistema Productivo.</p>
  </footer>
  <script>
    if (localStorage.getItem('modoEcoActivado') === 'true') {
      document.body.classList.add('modo-eco');
    }
    function toggleModoEco() {
      document.body.classList.toggle('modo-eco');
      localStorage.setItem('modoEcoActivado', document.body.classList.contains('modo-eco'));
    }
  </script>
</body>
</html>
```

proyecto.html 

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sobre el Proyecto</title>
  <link rel="stylesheet" href="./css/style.css">
  <link rel="icon" type="image/png" href="assets/favicon/favicon.png">
</head>
<body class="sobre-el-proyecto">
    <header>
        <h1>El Futuro es Verde</h1>
        <h2>Objetivos de Desarrollo Sostenible 2030</h2>
        <nav>
          <ul>
            <li><a href="index.html">Inicio</a></li>
            <li><a href="sostenibilidad.html">Sostenibilidad</a></li>
            <li><a href="proyecto.html">Sobre el Proyecto</a></li>
          </ul>
        </nav>

        <button onclick="toggleModoEco()" class="boton-eco">🌱 Modo Eco</button>
      </header>
  <main class="contenido-principal">
    <section class="propósito-proyecto">
      <h2 class="titulo-seccion">Propósito de esta web</h2>
      <p class="texto-seccion">Esta página ha sido desarrollada como parte de un proyecto educativo para la asignatura de Sostenibilidad aplicada al sistema productivo. El objetivo principal es demostrar cómo la tecnología puede ser utilizada de forma consciente y responsable con el medio ambiente, promoviendo la integración de soluciones tecnológicas sustentables en diferentes campos. El proyecto busca sensibilizar sobre el impacto ambiental de las infraestructuras tecnológicas y el papel crucial que juega la eficiencia energética en la construcción de un futuro más verde.</p>
      <p class="texto-seccion">El enfoque del proyecto es hacer que los usuarios tomen conciencia de los efectos negativos que tiene el consumo excesivo de energía y recursos en la tecnología actual, proponiendo alternativas y soluciones innovadoras para minimizar el impacto ambiental.</p>
    </section>

    <section class="infraestructura-proyecto">
      <h2 class="titulo-seccion">Infraestructura del Proyecto</h2>
      <p class="texto-seccion">El sitio está alojado en una Raspberry Pi 4, un microordenador de bajo consumo energético, que se utiliza para ejecutar el servidor web. Esta configuración permite comprobar cómo un servidor puede funcionar de manera eficiente y sostenible, en comparación con servidores tradicionales de gran consumo energético.</p>
      <p class="texto-seccion">La Raspberry Pi 4 ha sido elegida por su bajo consumo energético y su flexibilidad para ser utilizada en proyectos de sostenibilidad, siendo una excelente opción para usuarios que desean reducir su huella de carbono sin sacrificar el rendimiento. Además, este microordenador es capaz de ejecutar múltiples aplicaciones web, haciendo de este proyecto una prueba de concepto de cómo se pueden optimizar recursos tecnológicos sin comprometer la funcionalidad.</p>
      <p class="texto-seccion">En cuanto a la conectividad, el servidor está configurado para operar mediante una red local con bajo consumo de energía, lo que favorece la eficiencia en la transmisión de datos. La implementación de un servidor web tan ligero también contribuye a la reducción de residuos electrónicos, algo fundamental en el contexto del green computing.</p>
    </section>

    <section class="alimentacion-solar">
      <h2 class="titulo-seccion">Alimentación Solar</h2>
      <p class="texto-seccion">La Raspberry Pi funciona con energía 100% solar, proporcionada por una placa fotovoltaica instalada específicamente para este proyecto. Esta fuente de energía limpia y renovable garantiza que el servidor sea autosuficiente energéticamente, reduciendo considerablemente su huella de carbono. Gracias a esta instalación solar, el servidor funciona de manera completamente autónoma, sin la necesidad de energía proveniente de fuentes no renovables.</p>
      <p class="texto-seccion">El uso de energía solar no solo minimiza el impacto ambiental, sino que también asegura la continuidad de funcionamiento del sistema durante el día, mientras la placa fotovoltaica se recarga. Además, hemos utilizado una batería de almacenamiento de energía solar para garantizar que el servidor siga funcionando durante la noche o en días nublados, sin interrupciones.</p>
      <p class="texto-seccion">El proyecto demuestra cómo las energías renovables pueden ser integradas fácilmente en pequeños proyectos tecnológicos, llevando a cabo una transición a modelos de producción y consumo más responsables y respetuosos con el planeta.</p>
    </section>

    <section class="diseno-sostenible">
        <h2 class="titulo-seccion">Diseño Web Sostenible</h2>
        <p class="texto-seccion">Esta página ha sido diseñada con un enfoque minimalista, priorizando la simplicidad tanto en la estructura como en el estilo visual. Al evitar elementos innecesarios, efectos pesados o animaciones complejas, se ha logrado reducir significativamente el consumo de recursos del sistema, lo que se traduce en un menor impacto ecológico durante la navegación.</p>
        <p class="texto-seccion">El sitio utiliza una cantidad mínima de archivos y scripts, optimizados para garantizar tiempos de carga rápidos y un bajo uso de ancho de banda. Todas las imágenes han sido cuidadosamente seleccionadas y comprimidas sin perder calidad visual, reduciendo su tamaño para minimizar el uso de energía requerido al cargarlas en distintos dispositivos.</p>
        <p class="texto-seccion">Además, se ha evitado el uso de bibliotecas externas innecesarias, manteniendo el código limpio y ligero. Esta estrategia no solo mejora el rendimiento, sino que también contribuye a reducir la huella de carbono digital asociada al tráfico de datos. En conjunto, estas medidas hacen que esta web sea un ejemplo práctico de cómo se puede aplicar el diseño sostenible en proyectos reales.</p>
      </section>

    <section class="modo-eco">
      <h2 class="titulo-seccion">Modo Eco</h2>
      <p class="texto-seccion">Este sitio incluye un "modo eco" que reduce el uso de colores intensos y efectos visuales, optimizando aún más el consumo energético, especialmente en pantallas OLED y dispositivos móviles. Este modo está diseñado para ser activado por el usuario en la parte superior de la página o en el menú de navegación, de manera que aquellos usuarios que deseen reducir su impacto ambiental puedan hacerlo fácilmente.</p>
      <p class="texto-seccion">El "modo eco" también hace que el sitio sea más accesible para personas con dificultades visuales, ya que la simplicidad del diseño no solo reduce el uso de energía, sino que también mejora la legibilidad y la experiencia de navegación en diferentes dispositivos.</p>
      <p class="texto-seccion">En cuanto a la experiencia de usuario, hemos optimizado el diseño de las imágenes y los elementos multimedia del sitio para que se carguen rápidamente y consuman menos ancho de banda, lo que también contribuye a reducir el consumo energético a nivel global. El contenido de la web se presenta de forma clara y eficiente, sin sobrecargar el sistema ni los dispositivos de los usuarios.</p>
    </section>

    <section class="impacto-green-computing">
      <h2 class="titulo-seccion">Impacto del Green Computing</h2>
      <p class="texto-seccion">El green computing, o computación verde, es una práctica que busca el uso eficiente de los recursos tecnológicos, promoviendo el ahorro de energía, la reducción de desechos electrónicos y la integración de energías renovables. En este proyecto, hemos implementado varias optimizaciones de eficiencia energética tanto en el diseño de la web como en la infraestructura del servidor.</p>
      <p class="texto-seccion">Una de las principales ventajas del green computing es que permite reducir significativamente el consumo de recursos energéticos en el sector tecnológico, que es uno de los principales responsables de las emisiones de gases de efecto invernadero. Además, la optimización de la gestión de residuos electrónicos es un factor clave para mitigar la creciente acumulación de desechos en el planeta.</p>
      <p class="texto-seccion">Además, la implementación de soluciones como la energía solar, la eficiencia en el diseño web y el uso de dispositivos como la Raspberry Pi está demostrando que se puede tener un impacto positivo en la sostenibilidad sin comprometer el rendimiento o la funcionalidad. Este proyecto actúa como un modelo a seguir para otros desarrolladores, empresas y organizaciones que deseen incorporar prácticas de green computing en sus operaciones diarias.</p>
    </section>

    <section class="perspectivas-futuras">
      <h2 class="titulo-seccion">Perspectivas Futuras</h2>
      <p class="texto-seccion">Este proyecto tiene el objetivo de inspirar a otros a explorar formas innovadoras de aplicar la sostenibilidad en el campo de la tecnología. En el futuro, se planea extender el uso de energía solar para alimentar otros dispositivos en la infraestructura tecnológica, así como realizar un análisis exhaustivo de la eficiencia energética del servidor web.</p>
      <p class="texto-seccion">También se planea implementar nuevas funcionalidades en el sitio, como la integración de sistemas de monitoreo energético en tiempo real, para que los usuarios puedan visualizar el impacto de su navegación en el consumo de energía. De esta manera, el proyecto continuará evolucionando como una plataforma educativa sobre sostenibilidad, accesible para estudiantes, desarrolladores y cualquier persona interesada en las tecnologías verdes.</p>
    </section>

    <section class="autores">
        <p>Autores: Abel Suazo, Juan Herrador, Sergio Aragón, Francisco Alba</p>
      </section>
    
  </main>

  <footer class="footer-proyecto">
    <p class="texto-footer">Diseño sostenible, tecnología responsable. Proyecto educativo con impacto real.</p>
  </footer>
  <script>
    if (localStorage.getItem('modoEcoActivado') === 'true') {
      document.body.classList.add('modo-eco');
    }
  
    function toggleModoEco() {
      document.body.classList.toggle('modo-eco');
      localStorage.setItem('modoEcoActivado', document.body.classList.contains('modo-eco'));
    }
  </script>
</body>
</html>
```

sostenibilidad.html 

```html
<!-- sostenibilidad.html -->
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sostenibilidad</title>
  <link rel="stylesheet" href="./css/style.css">
  <link rel="icon" type="image/png" href="assets/favicon/favicon.png">
</head>
<body>
    <header>
        <h1>El Futuro es Verde</h1>
        <h2>Objetivos de Desarrollo Sostenible 2030</h2>
        <nav>
          <ul>
            <li><a href="index.html">Inicio</a></li>
            <li><a href="sostenibilidad.html">Sostenibilidad</a></li>
            <li><a href="proyecto.html">Sobre el Proyecto</a></li>
          </ul>
        </nav>

        <button onclick="toggleModoEco()" class="boton-eco">🌱 Modo Eco</button>
      </header>
  <main class="sostenibilidad-main">
    <section class="sostenibilidad-seccion" id="desarrollo-sostenible">
        <h2>¿Qué es el desarrollo sostenible?</h2>
        <p>El desarrollo sostenible es un concepto que ha evolucionado a lo largo del tiempo y se refiere a un modelo de desarrollo que tiene en cuenta no solo el crecimiento económico, sino también la protección del medio ambiente y el bienestar social. Esto significa que debemos encontrar un equilibrio entre las necesidades presentes y las futuras, asegurándonos de no agotar los recursos naturales ni causar daño irreversible a los ecosistemas. Las políticas de desarrollo sostenible promueven la utilización de recursos renovables y la minimización de residuos, para que las futuras generaciones puedan disfrutar de los mismos recursos y calidad de vida.</p>
        <p><a href="https://es.wikipedia.org/wiki/Desarrollo_sostenible" class="more-info-link">+ Más info</a></p>
      </section>
      
      <section class="sostenibilidad-seccion" id="biodiversidad">
        <h2>Biodiversidad</h2>
        <p>La biodiversidad es uno de los pilares más importantes de la sostenibilidad global. Esta se refiere a la variedad de vida en la Tierra, desde las especies animales y vegetales hasta los ecosistemas que las albergan. La pérdida de biodiversidad afecta gravemente la seguridad alimentaria, la salud humana, y los procesos ecológicos vitales como la polinización y la purificación del aire. Para proteger la biodiversidad, es fundamental reducir la destrucción de hábitats naturales, promover la agricultura sostenible y crear reservas naturales que sirvan como refugios para especies en peligro de extinción.</p>
        <p><a href="https://es.wikipedia.org/wiki/Biodiversidad" class="more-info-link">+ Más info</a></p>
      </section>
      
      <section class="sostenibilidad-seccion" id="plastico">
        <h2>Contaminación por plásticos</h2>
        <p>La contaminación por plásticos es uno de los mayores desafíos medioambientales que enfrentamos hoy en día. Cada año, millones de toneladas de plástico terminan en los océanos, afectando gravemente a la fauna marina y contaminando los ecosistemas acuáticos. Los plásticos no solo son perjudiciales para los animales, que los confunden con alimento, sino que también pueden ingresar a la cadena alimentaria humana. Para combatir esta problemática, se están promoviendo alternativas biodegradables, la reducción del consumo de plásticos de un solo uso, y el reciclaje eficiente. Es fundamental que todos adoptemos prácticas más responsables en nuestro uso del plástico.</p>
        <p><a href="https://es.wikipedia.org/wiki/Contaminaci%C3%B3n_por_pl%C3%A1sticos" class="more-info-link">+ Más info</a></p>
      </section>
      
      <section class="sostenibilidad-seccion" id="consumo-energetico">
        <h2>Consumo energético digital</h2>
        <p>En la era digital, el consumo energético está creciendo rápidamente debido a la expansión de dispositivos electrónicos y la necesidad de servidores para almacenar y procesar información. Cada búsqueda en línea, cada mensaje enviado o cada video visto consume energía, muchas veces de fuentes no renovables. El sector tecnológico, al igual que otros, tiene la responsabilidad de reducir su huella energética. La adopción de energías renovables, la eficiencia energética y el diseño sostenible de dispositivos son algunas de las formas en que podemos contribuir a un futuro más verde. El Green Computing es un enfoque que promueve prácticas digitales sostenibles.</p>
        <p><a href="https://es.wikipedia.org/wiki/Energ%C3%ADa_digital" class="more-info-link">+ Más info</a></p>
      </section>
      
      <section class="sostenibilidad-seccion" id="green-computing">
        <h2>Green Computing</h2>
        <p>Green Computing o computación verde es una filosofía que promueve la reducción del impacto ambiental de los sistemas informáticos. Este enfoque busca mejorar la eficiencia energética de los dispositivos y minimizar el uso de materiales peligrosos, así como promover el reciclaje. Desde la fabricación de computadoras hasta el uso cotidiano de las tecnologías, Green Computing busca optimizar el rendimiento sin comprometer el medio ambiente. Iniciativas como la virtualización de servidores, la adopción de energías renovables en centros de datos, y la creación de productos electrónicos con menor impacto ambiental están ganando terreno.</p>
        <p><a href="https://es.wikipedia.org/wiki/Computaci%C3%B3n_verde" class="more-info-link">+ Más info</a></p>
      </section>
  </main>

  <footer>
    <p>Conocimiento para un futuro sostenible. Web ligera diseñada con eficiencia energética.</p>
  </footer>
  <script>
    if (localStorage.getItem('modoEcoActivado') === 'true') {
      document.body.classList.add('modo-eco');
    }
    function toggleModoEco() {
      document.body.classList.toggle('modo-eco');
      localStorage.setItem('modoEcoActivado', document.body.classList.contains('modo-eco'));
    }
  </script>
</body>
```

style.css

```css
/* General Variables */
:root {
  --bg-color: #fffef7;      /* Color de fondo claro (color beige) */
  --text-color: #283618;    /* Color de texto oscuro (color verde oliva oscuro) */
  --accent-color: #dda15e;  /* Color de acento (color mostaza) */
  --header-color: #9dba3e;  /* Color para el encabezado (verde oliva) */
  --eco-bg-color: #242424; /* Fondo para secciones relacionadas con la ecología (blanco) */
  --eco-text-color: #333;   /* Color de texto para la ecología (gris oscuro) */
  --pastel-green: #21241e;  /* Verde pastel para los elementos de diseño */
  --card-green: #b2bea1;
  --pastel-brown: #7b6c5e;  /* Marrón pastel para el efecto de gradiente */
}

body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background-color: var(--bg-color);
  color: var(--text-color);
  line-height: 1.6;
  transition: background-color 0.3s, color 0.3s;
}

/* === Footer === */
footer {
  background-color: #e3e3e3;
  text-align: center;
  padding: 1rem;
  font-size: 0.9rem;
  color: #444;
  position: relative; /* Asegura que el footer se quede al final */
  z-index: 2; /* Está por encima del contenido */
}

footer p {
  margin: 0;
}

header {
  background: linear-gradient(135deg, var(--pastel-green), var(--pastel-brown));
  color: white;
  padding: 1.5rem 2rem;
  font-family: 'Arial', sans-serif;
  display: flex;
  flex-direction: column;
  align-items: flex-start; /* Alinea todo a la izquierda */
}

header h1 {
  font-family: 'Poppins', sans-serif;
  font-size: 3rem;
  font-weight: 700;
  color: white;
  text-transform: uppercase;
  letter-spacing: 2px;
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);
  margin: 0;
}

header h2 {
  font-family: 'Poppins', sans-serif;
  font-size: 1.2rem;
  color: white;
  margin: 0px;
  margin-bottom: 20px;
}

nav {
  background-color: #666d56;
  border-radius: 20px;
  padding: 5px 15px;
  margin-top: 0.5rem;
}

nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  gap: 2rem;
}

nav a {
  color: white;
  text-decoration: none;
  font-size: 1rem;
  text-transform: uppercase;
  transition: transform 0.3s ease, color 0.3s ease;
}

nav a:hover {
  color: var(--accent-color);
  transform: translateY(-2px);
}

.boton-eco {
  background-color: var(--accent-color);
  color: var(--text-color);
  border: none;
  padding: 0.5rem 1rem;
  font-weight: bold;
  cursor: pointer;
  border-radius: 8px;
  transition: all 0.3s ease;
  margin-top: 1rem;
}

.boton-eco:hover {
  background-color: var(--header-color);
  color: var(--eco-bg-color);
}

/* === Sección de Bienvenida (Intro) === */
section.intro {
  position: relative;
  background-image: url('../assets/comprimidas/warming-green-forest.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  padding: 3rem 2rem;
  color: white; /* Texto en blanco */
  text-align: center;
  filter: grayscale(40%); /* Desatura la imagen */
  height: 50vh; /* Ajusta la altura para no ser tan grande */
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.intro h2 {
  font-size: 4rem;
}

.intro p {
  font-size: 1.4rem;
}

section.intro::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.3); /* Overlay oscuro semitransparente */
  z-index: -1; /* Coloca el overlay debajo del contenido */
}

h2 {
  font-size: 2.5rem;
  z-index: 1; /* Asegura que el título esté por encima del overlay */
}

p {
  font-size: 1.1rem;
  z-index: 1; /* Asegura que el párrafo esté por encima del overlay */
}

/* === Sección de Objetivos de Desarrollo Sostenible (ODS) === */
.ods {
  padding: 2rem;
  background-color: var(--bg-color);
}

.ods h2 {
  text-align: center;
  font-size: 2rem;
  margin-bottom: 2rem;
}

.cards-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
}

/* === Estilo de cada tarjeta === */
.card summary {
  background-color: var(--card-green);
  padding: 1rem 1.2rem;
  font-weight: bold;
  font-size: 1.1rem;
  cursor: pointer;
  color: var(--text-color);
  list-style: none;
  border-bottom: 1px solid #c2dec4;
  transition: background-color 0.3s ease;
}

.card summary:hover {
  background-color: --;
}

.card p {
  padding: 1rem 1.2rem;
  font-size: 0.95rem;
  color: #333;
  text-align: justify;
}

.card {

  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.08);
  overflow: hidden;
  position: relative;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

/* Efecto hover */
.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.1);
}

/* === Estilo para difuminar el fondo === */
.card input[type="radio"] {
  display: none;
}

.card input[type="radio"]:checked + details {
  filter: none; /* Cuando está seleccionado, no hay filtro */
}

.card input[type="radio"]:not(:checked) + details {
  filter: blur(3px); /* Difumina el fondo de los detalles no seleccionados */
}

.card input[type="radio"]:checked + details {
  transform: scale(1.05); /* Se puede aumentar el tamaño del detalle seleccionado */
}

/* Mejoras visuales para dispositivos pequeños */
@media (max-width: 600px) {
  .ods h2 {
    font-size: 1.5rem;
  }

  .card summary {
    font-size: 1rem;
  }

  .card p {
    font-size: 0.9rem;
  }
}

/* Estilos específicos para la página de sostenibilidad */
.sostenibilidad-main {
  padding: 0 2rem;
}

.sostenibilidad-seccion {
  background-size: cover;
  background-position: center;
  padding: 4rem;
  margin: 2rem 0;
  color: white;
  border-radius: 8px;
  position: relative;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* Crear overlay oscuro para mejorar el contraste */
.sostenibilidad-seccion::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.4); /* Ajusta la opacidad para mayor o menor contraste */
  border-radius: 8px;
  z-index: 1; /* Asegura que el overlay esté encima de la imagen, pero debajo del texto */
}

.sostenibilidad-seccion h2 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
  z-index: 2; /* Asegura que el texto esté encima del overlay */
  position: relative; /* Necesario para que el z-index funcione */
}

.sostenibilidad-seccion p {
  text-align: justify;
  font-size: 1.1rem;
  line-height: 1.8;
  max-width: 800px;
  margin: 0 auto;
  z-index: 2; /* Asegura que el texto esté encima del overlay */
  position: relative; /* Necesario para que el z-index funcione */
}

/* Opcional: Sombra de texto para mejorar aún más la legibilidad */
.sostenibilidad-seccion h2, .sostenibilidad-seccion p {
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5); /* Sombra de texto */
}

#desarrollo-sostenible {
  background-image: url('../assets/comprimidas/landscape1.png');
}

#biodiversidad {
  background-image: url('../assets/comprimidas/landscape3.png');
}

#plastico {
  background-image: url('../assets/comprimidas/landscape2.png');
}

#consumo-energetico {
  background-image: url('../assets/comprimidas/landscape5.jpg');
}

#green-computing {
  background-image: url('../assets/comprimidas/green-computing.jpg');
}

/* Filtro oscuro para hacer el texto más legible */
.sostenibilidad-seccion::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  border-radius: 8px;
  pointer-events: none; /* Permite interactuar con el contenido detrás */
}

/* Estilos para el enlace "+ Más info" */
.more-info-link {
  display: inline-block;
  margin-top: 1rem;
  color: var(--primary-color); /* Puedes definir un color específico */
  font-weight: bold;
  text-decoration: none;
  font-size: 1.1rem;
  transition: color 0.3s ease, transform 0.3s ease;
}

.more-info-link:hover {
  color: var(--accent-color); /* Cambio de color al pasar el cursor */
  transform: translateY(-2px);  /* Efecto de elevarse */
}

/* Añadir espacio entre el enlace y el resto del contenido */
.sostenibilidad-seccion p {
  margin-bottom: 1.5rem;
}

/* Estilos solo para la página 'Sobre el Proyecto' */
body.sobre-el-proyecto {
  font-family: 'Segoe UI', sans-serif;
  line-height: 1.6;
  background-color: var(--bg-color);
  color: var(--text-color);
  margin: 0;
  padding: 0;
}

/* Contenido principal */
.contenido-principal {
  padding: 1rem 3rem;
  background-color: var(--bg-color);
  color: var(--eco-text-color);
}

.titulo-seccion {
  color: var(--text-color);
  margin-top: 2rem;
  margin-bottom: 1rem;
  font-size: 1.8rem;
  border-bottom: 2px solid var(--accent-color);
  padding-bottom: 0.3rem;
}

.texto-seccion {
  text-align: justify;
  margin-bottom: 1rem;
  color: var(--eco-text-color);
}

.autores {
  text-align: center;
  font-size: 0.9rem;
  color: #777;  /* Gris claro para que no destaque demasiado */
  margin-top: 3rem;
}

.autores p {
  margin: 0;
}

.boton-eco {
  background-color: var(--accent-color);
  color: var(--text-color);
  border: none;
  padding: 0.5rem 1rem;
  font-weight: bold;
  cursor: pointer;
  border-radius: 8px;
  transition: all 0.3s ease;
  position: absolute;
  top: 1rem;
  right: 1rem;
}

.boton-eco:hover {
  background-color: var(--header-color);
  color: var(--eco-bg-color);
}

body.modo-eco {
  filter: brightness(0.82) saturate(0.8); /* Aplica a todo lo visual dentro del body */
  color: var(--text-color); /* Mantén color de texto legible */
}
```


Inicio -> **[Volver al inicio ](README.md)**  
Anterior -> **[Presupuesto](precio.md)**  
Siguiente -> **[Referencias](#referencias)** 
