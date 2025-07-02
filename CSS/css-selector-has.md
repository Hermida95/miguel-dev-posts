# 🧵 Selector `:has()` en CSS

📅 Publicado en LinkedIn el 1 de julio de 2025  
✍️ Autor: Miguel García Hermida  
🔗 [Ver publicación en LinkedIn](https://www.linkedin.com/in/miguel-garcía-hermida-796b67180/)

---

🎯 ¿Sabías que en CSS puedes detectar si un elemento tiene hijos o no?

A veces queremos cambiar el estilo de un contenedor solo si está vacío (por ejemplo, mostrar un mensaje o cambiar el fondo si aún no hay contenido).

Con :has() + :empty podemos hacerlo de forma elegante:

.card:has(:empty) {
  background-color: #f8d7da;
  border: 2px dashed #f5c2c7;
  text-align: center;
  content: "Aún no hay contenido";
}

🔍 Esto significa que si un <article> contiene una <img>, se le aplica un borde.
Antes necesitábamos JavaScript para esto. Ahora, ¡CSS se pone listo!
article:has(img) {
  border: 2px solid #4ade80;
}

🧠 Ideal para mejorar la accesibilidad, UX y diseño responsive con menos código.


💡 Lo interesante:

:has() te permite seleccionar un elemento padre según lo que contiene dentro.
Es CSS puro, sin necesidad de JavaScript para comprobar si hay elementos hijos.
Muy útil en apps dinámicas o SPA donde se cargan cosas con JavaScript o React/Vue.
⚠️ Eso sí, todavía no es compatible con todos los navegadores (especialmente Firefox), pero ya funciona en Chrome y Safari. ¡Así que es un buen momento para empezar a probarlo!
