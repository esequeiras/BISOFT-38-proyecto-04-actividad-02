<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->

# BISOFT-38 Proyecto de Ingeniería del Software 4

_Este repositorio nos ayudará a introducir el concepto de Mobile testing_

</header>

<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  TBD-step-2-notes.
-->

## Paso 2: Agregar el código funcional

_Con el proyecto creado, ahora vamos a agregar código funcional_

### :keyboard: Actividad: Paso 02

1. Inicia Android Studio.
1. En el directorio `commonMain/kotlin`, crea un nuevo directorio `common.example.search`.
1. En este directorio, crea un archivo Kotlin, `Grep.kt`, y agrega la siguiente función:
    ```kotlin
    fun grep(lines: List<String>, pattern: String, action: (String) -> Unit) {
      val regex = pattern.toRegex()
      lines.filter(regex::containsMatchIn)
        .forEach(action)
    }
    ```
    Esta función está diseñada para parecerse al [comando grep de UNIX](https://es.wikipedia.org/wiki/Grep). Aquí, la función toma líneas de texto, un patrón utilizado como una expresión regular y una función que se invoca cada vez que una línea coincide con el patrón.
1. Sube los cambios haciendo un commit de los archivos y push a la rama main.
1. Espera unos 20 segundos y luego actualiza esta página (la que estás siguiendo las instrucciones). [GitHub Actions](https://docs.github.com/es/actions) se actualizará automáticamente al siguiente paso.


