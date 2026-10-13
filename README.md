# Mi primer proyecto Android

Pantalla de bienvenida que cumple los tres puntos de la tarea.

## 1. Cuatro idiomas

| Idioma | Archivo |
|---|---|
| Español (por defecto) | `app/src/main/res/values/strings.xml` |
| Inglés | `app/src/main/res/values-en/strings.xml` |
| Francés | `app/src/main/res/values-fr/strings.xml` |
| Alemán | `app/src/main/res/values-de/strings.xml` |

La app toma el idioma del dispositivo; cualquier otro idioma cae en español.

## 2. Fondo nine-patch

`app/src/main/res/drawable-xhdpi/fondo.9.png` es la imagen de la tarea con sus
marcas nine-patch. Solo se estira el cielo a la izquierda, a la derecha y
encima del androide, por lo que este no se deforma al redimensionar.

## 3. Múltiples pantallas

Un solo layout con `ConstraintLayout` (`res/layout/activity_main.xml`) cuyas
medidas se adaptan con recursos alternativos:

- `values/dimens.xml`: teléfonos en vertical
- `values-land/dimens.xml`: teléfonos en horizontal
- `values-sw600dp/dimens.xml`: tabletas de 7"
- `values-sw720dp/dimens.xml`: tabletas de 10" y pantallas grandes

## Cómo ejecutarlo

Abrir la carpeta en Android Studio y pulsar **Run**. Requiere JDK 17 para Gradle.
