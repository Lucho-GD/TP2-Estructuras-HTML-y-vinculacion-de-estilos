# Reflexión - Laboratorio 2

## Imagen y atributo alt

El nombre de la imagen que guardé dentro de la carpeta `img/` es:

`img-mifoto.jpg`

El atributo `alt` utilizado en la etiqueta `<img>` es:

`Foto de Luciano Garcia Diaz`

## Importancia de las etiquetas semánticas

Es fundamental utilizar etiquetas semánticas como `<main>`, `<nav>`, `<header>`, `<section>`, `<article>` y `<footer>` porque permiten definir claramente la función de cada parte de una página web.

A diferencia de utilizar únicamente etiquetas `<div>`, las etiquetas semánticas aportan significado a la estructura del documento. Esto facilita la comprensión del código, mejora la accesibilidad para usuarios que utilizan lectores de pantalla y también ayuda a los motores de búsqueda a interpretar mejor el contenido del sitio.

## Verificación de las rutas

Para comprobar que las rutas de los enlaces eran correctas, primero abrí los archivos HTML directamente desde mi PC y probé los enlaces "Inicio" y "Acerca de" para verificar que ambas páginas se pudieran abrir correctamente.

Luego subí los archivos al repositorio de GitHub y desplegué el proyecto mediante GitHub Pages. Desde la página publicada volví a probar los enlaces de navegación para comprobar que funcionaran correctamente también ahí.


# Reflexión - Laboratorio 3

## 1. Código Postal

Para el campo de Código Postal utilicé este código:

```html
<input type="text" id="codigo-postal" name="codigo-postal"
       pattern="^[A-Z]\d{4}[A-Z]{3}$"
       title="Ingrese un código postal con el formato A1234ABC"
       required>
```

El `pattern` sirve para indicar qué formato tiene que tener el código postal. En este caso, tiene que empezar con una letra mayúscula, seguir con cuatro números y terminar con tres letras mayúsculas. El `title` muestra una indicación sobre el formato que se tiene que ingresar.

## 2. Etiqueta `<label>`

La etiqueta `<label>` sirve para ponerle un nombre o indicar qué se tiene que ingresar en un campo del formulario.

Para relacionarla con un campo se usa `for` en el `label` y tiene que ser igual al `id` del campo. Por ejemplo:

```html
<label for="codigo-postal">Código Postal:</label>
<input type="text" id="codigo-postal" name="codigo-postal">
```

De esta forma, el texto "Código Postal" queda asociado a ese campo.

## 3. Campos de tipo radio

Los campos `radio` sirven para elegir una opción entre varias.

Si cada `radio` tiene un `name` diferente, se pueden seleccionar varias opciones porque cada uno pertenece a un grupo distinto.

En cambio, si tienen el mismo `name`, forman parte del mismo grupo y solamente se puede seleccionar una opción.

Por ejemplo:

```html
<input type="radio" name="contacto" value="correo">
<input type="radio" name="contacto" value="postal">
<input type="radio" name="contacto" value="telefono">
```

En este caso, solamente se puede elegir una de las tres opciones.
