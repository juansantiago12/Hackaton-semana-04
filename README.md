1.- ESLint

    ESLint es una herramienta de código abierto enfocado en revisar, observar y busca errores que puedan afectar tu código para javascript (o más correctamente para ECMAScript). ESLint es la herramienta predominante para la tarea de "limpiar" código javascript tanto en el servidor como en el navegador.
    Esta herramienta nos puede ayudar a:

    -Mostrarte errores de sintaxis.
    -Mostrarte errores cuando no se siguen buenas prácticas.
    -Proveer sugerencias para mejorar tu código.
    -Mantener un estilo consistente en tu código o reforzar reglas internas de tu propio equipo.

2.  Prettier

    Prettier se utiliza para formatear automáticamente tu código, soportando la sintaxis de una gran cantidad de lenguajes, entre los que están JavaScript, JSX, Flow, TypeScript, JSON, HTML, Vue, Angular, CSS, Less, SCSS, GraphQL, MarkDown, CommonMark, MDX y YAML.
    Además, mediante varios plugins también soporta Apex, Elm, Java, PHP, PostgreSQL, Ruby, Swift, TOML y XML, entre otros.
    Prettier actualmente dispone de integraciones para los editores de texto e IDEs más utilizados, como por ejemplo VS Code, Visual Studio, Atom, Sublime, Vim, Emacs, PHPStorm o WebStorm.

    Funcionalidad de Prettier:

    Prettier es usado para que todo el código siga un mismo estilo la cual facilita que las personas que se inician en este lenguaje se adapten a usar una notación concreta para nombres de variables o funciones o formatos de código como la creación de sangrías al comienzo de cada línea mediante espacios en lugar de pulsar el tabulador, mezcla de comillas simples y dobles, ajuste de paréntesis opcionales que rodean el parámetro de la función de flecha entre otros.

    Instalación y configuración de Prettier en VS Code:

        1.- Abre la paleta de extensiones pulsando CTRL+SHIFT+x en Windows.
        2.- Busca «Extensions: Install Extensions» y haz clic en dicha opción cuando aparezca.
        3.- Introduce Prettier en el campo de búsqueda y haz clic «Prettier – Code formatter» para instalarlo.
        4.- Cuando la instalación finalice, cierra VS Code y vuelve a abrirlo.
        5.- Una vez instales Prettier bastará con que selecciones la opción Format Document en el menú que puedes desplegar haciendo clic derecho en el editor o pulsando CTRL+SHIFT+p para aplicar los formatos.
        6.- Para poder configurar los diferentes parámetros de Prettier nos podemos dirigir al siguiente enlace https://prettier.io/playground/ una ves establecidas nuestras preferencias lo copiamos nos dirigimos a VS Code, Manage, Settings y luego a Open Setting UI para agregar nuestro código.
        7.- Una de las principales configuraciones es de que el formato de código se realice de forma automática agregando el siguiente código:
        “editor.formatOnSave”: true

3.- EditorConfig

    EditorConfig es un archivo de configuración en el que definimos todas estas características, de forma genérica o filtrando según la extensión del archivo, y que se deposita junto con el proyecto. De esta forma, a cualquiera que trabaje sobre el proyecto, se le aplicará automáticamente la configuración sin alterar la propia de su editor. Tan solo tendremos que instalar una extensión si el editor que usamos no es uno de los que lo traen por defecto instalado consultándolo en la lista de editores soportados.

    Funcionamiento:

    -Creamos un archivo. editorconfig que guardaremos en el directorio raíz de nuestro proyecto.
    -Lo editamos para añadir la configuración que deseemos. Por ejemplo lo podemos configurar de que utilice el fin de línea de Unix, una codificación de caracteres en UTF-8 y que la indentación sea con 2 espacios.

        # top-most EditorConfig file
        root = true
        # Unix-style newlines with a newline ending every file
        [*]
        end_of_line = lf
        insert_final_newline = true
        # Matches multiple files with brace expansion notation
        # Set default charset
        [*.{html,css,js}]
        charset = utf-8
        # 2 space indentation
        [*.{html,css,js}]
        indent_style = space
        indent_size = 2

    -La próxima vez que abramos cualquier archivo del proyecto, aunque se hubiera guardado con una configuración diferente, se nos mostrará en nuestro editor con la configuración establecida.
