# README – Práctica Calificada N.º 3: Hojas de Estilo en Cascada

**Alumno:** Rodrigo Nicolas Franco Gutierrez · **Código:** U24244377
**Docente:** Antonio Arroyo Paz
**Curso:** 1000005158 – Hojas de Estilo en Cascada (UTP, Arequipa) · Sección 47318 · Aula BS109
**Fecha:** 29 de octubre de 2026

## Uso de IA
El docente autorizó el uso de IA para esta práctica. Se utilizó **Claude (Anthropic)** para generar el código. Este archivo documenta el prompt usado.

## Prompt utilizado
Se adjuntó una foto del enunciado del examen y se escribió:

> haz todo, el profesor nos dijo que usemos ia y hagamos un readme aparte con el prompt, necesito que el trabajo se pueda entregar con un link y se visualice cada pregunta, los colores para decorar son rojo, negro y azul, digamos una pregunta con la página rojo y negro y la otra con azul y negro y así sucesivamente.

### Enunciado transcrito (foto adjunta)
1. **Pregunta 1 (5 pts):** Diseña una pequeña interfaz de tu elección (menú de navegación, lista de tarjetas de productos, botonera, formulario de contacto, etc.) en la que los elementos interactivos respondan al usuario con transiciones suaves.
2. **Pregunta 2 (5 pts):** Crea una galería o conjunto de tarjetas (personajes, destinos turísticos, cursos o recetas) que utilice transformaciones para generar efectos visuales atractivos al interactuar con ellas.
3. **Pregunta 3 (5 pts):** Diseña un elemento animado de tu elección (loader original, mascota o personaje animado con formas CSS, fondo en movimiento, reloj, paisaje con elementos que se mueven, etc.) que se ejecute por sí mismo, sin necesidad de interacción.
4. **Pregunta 4 (5 pts):** Crea una página o componente (panel con efecto de vidrio, galería en rejilla o tarjeta de perfil) que utilice propiedades modernas de CSS y que siga funcionando correctamente en navegadores que no las soportan. Requisitos mínimos:
   - Al menos una regla `@supports` con una alternativa (base funcional + mejora).
   - Al menos 2 propiedades con valores de reserva (fallbacks) o con prefijos de proveedor correctamente ordenados (el estándar al final).
   - Un bloque `@media (prefers-reduced-motion: reduce)` que reduzca o desactive las animaciones.
   - Comentario CSS o archivo de compatibilidad breve con el resultado de pruebas en dos navegadores y la fuente consultada (caniuse.com o MDN).

## Resultado
Una sola página (`practica-css-3.html`) con las 4 preguntas, navegables desde una barra superior:

| Pregunta | Tema | Paleta |
|---|---|---|
| 1 | Interfaz: menú, tarjetas, botones, formulario | Rojo y negro |
| 2 | Galería de destinos turísticos con tarjetas 3D | Azul y negro |
| 3 | Reloj animado con formas CSS (autónomo) | Rojo y negro |
| 4 | Paneles de vidrio con `@supports`, fallbacks y tabla de compatibilidad | Azul y negro |

## Notas
- Solo HTML y CSS; un script mínimo en la P3 solo sincroniza el reloj con la hora actual.
- Se incluye `prefers-reduced-motion` en las animaciones y transiciones.
- Las pruebas de compatibilidad de la P4 deben confirmarse abriendo la página en dos navegadores (por ejemplo Chrome y Firefox).

## Estructura del proyecto
```
index.html          Portada con acceso a las 4 preguntas
pregunta1.html      Interfaz interactiva (rojo y negro)
pregunta2.html      Galería turística (azul y negro)
pregunta3.html      Elemento animado (rojo y negro)
pregunta4.html      Glassmorphism + @supports (azul y negro)
base.css            Estilos comunes: variables, header, pie, portada
p1.css ... p4.css      Estilos de cada pregunta
compatibilidad.txt  Resultado de pruebas y fuentes (Pregunta 4)
```
Cada página comparte un header fijo con botones de navegación (menú hamburguesa en celular) y botones Anterior/Siguiente al final.
