1. Herramienta elegida
Descripción:

ChatGPT (GPT-4o) y DeepSeek. Elegí esta herramienta porque su capacidad para procesar contexto largo y generar código HTML/CSS/JS limpio en un solo bloque facilita el Vibe Coding. Además, su habilidad para explicar errores técnicos en lenguaje sencillo fue clave para la fase de depuración.

2. Definición del Tema
"Tierra Viva" - Venta de terrenos en México. El propósito de la página es ofrecer una experiencia de usuario premium, minimalista y altamente informativa para personas interesadas en comprar terrenos para inversión o construcción en México. El sitio incluye datos reales del mercado, opciones de financiamiento, advertencias legales y un cotizador dinámico.

3. Prompt Estructurado
Rol: Diseñador UI/UX y Desarrollador Frontend Senior.
Tarea: Crear una landing page completa de venta de terrenos llamada "Tierra Viva".
Contexto: El sitio debe verse como una revista de arquitectura de alta gama (estilo minimalista, asimétrico, con efecto glassmorphism). Debe incluir secciones de mercado en México, precios por m², seguridad legal y un cotizador interactivo.
Restricciones: Usar tipografía Playfair Display e Inter. Debe ser 100% responsive. Implementar un Modo Oscuro funcional con persistencia (localStorage) que mantenga el contraste en todas las secciones. Todo el código debe estar en un solo archivo (HTML, CSS y JS).

4. Pruebas y Funcionalidad
Realicé pruebas manuales:
Navegación: Los enlaces internos del menú superior (Mercado, Precios, Legal) hacen scroll suavemente a las secciones.
Modo Oscuro: El botón 🌙/☀️ alterna los colores correctamente. Al recargar la página, la preferencia se guarda y respeta. La sección de precios mantiene su contraste en ambos modos.
Interactividad (Cotizador): Al hacer clic en "Cotizar" o "Ver Disponibilidad", la ventana modal se abre correctamente. El botón "X" la cierra. El botón "Calcular Total" ejecuta la operación matemática y formatea el resultado con comas.

5. Corrección de Errores
Error encontrado: Al dejar el campo de "Metros cuadrados" vacío o escribir letras, el cotizador arrojaba NaN (Not a Number) en pantalla, rompiendo la lógica visual.
Solución con IA: Le consulté a la IA: "¿Qué salió mal y cómo lo arreglo?". La IA explicó que debía convertir el valor de texto a número con parseFloat y crear una "guardia de seguridad" con isNaN (Si no es un número, muestra alerta).
Aprendizaje: Comprendí que los inputs del usuario son datos "sucios" y siempre deben validarse y convertirse antes de realizar operaciones matemáticas.

6. Link del Repositorio (GitHub)
[Github](https://github.com/sinbriz/Tierra_Viva)

7. Documentación README
# Tierra Viva - Venta de Terrenos en México 
Este proyecto es una landing page desarrollada con **Vibe Coding**, diseñada para la venta de terrenos en México. Cuenta con un diseño premium minimalista, modo oscuro y un cotizador interactivo.

## Herramientas Usadas
- **IA:** ChatGPT y DeepSeek (Generación de código y depuración)
- **Frontend:** HTML5, CSS3 (Variables, Flexbox, Grid, Glassmorphism)
- **JavaScript:** Lógica del cotizador, Modo Oscuro (LocalStorage) y ventana modal.
- **Tipografías:** Google Fonts (Playfair Display e Inter).

## Funcionalidades
- Diseño responsive (adaptable a celulares).
- Modo oscuro persistente (recuerda la elección del usuario).
- Cotizador dinámico de terrenos con validación de errores.
- Información actualizada del mercado de terrenos en México (precios, financiamiento y legalidad).

## Prompts Destacados
- *Prompt inicial:* "Crea una landing page de venta de terrenos estilo revista de arquitectura, con modo oscuro, fondo de paisaje y tarjeta con efecto glassmorphism. Usa Playfair Display..."
- *Prompt de corrección:* "Mi cotizador arroja NaN cuando el usuario no escribe nada. ¿Qué salió mal y cómo lo arreglo?"

## Enlace al sitio publicado
[Ver sitio en vivo aquí](https://stellular-dasik-79773b.netlify.app/)
8. Link de la Página Publicada
[Sitio]((https://stellular-dasik-79773b.netlify.app/))
