# Minuta de la Sesión de Adultos - Conferencia de Estaca

Este proyecto es una página web simple que muestra la minuta (el programa) para la sesión de adultos de la Conferencia de Estaca. Está diseñada para ser fácil de visualizar y modificar.

## Estructura de Archivos

El proyecto tiene una estructura sencilla:

```
.
├── index.html       # El archivo principal con todo el contenido y la estructura.
├── css/
│   └── style.css    # Archivo de estilos para cambiar la apariencia (colores, fuentes, etc.).
└── images/
    ├── lds-logo.png # Logo de la Iglesia.
    └── logo.png     # Logo de la estaca o del evento.
```

## ¿Cómo modificar la minuta?

No se necesita conocimiento avanzado de programación para realizar cambios básicos. Solo necesitas un editor de texto simple (como el Bloc de Notas, VS Code, Sublime Text, etc.).

### 1. Modificar el Contenido (Textos)

Todo el texto visible en la página se encuentra en el archivo `index.html`.

1.  Abre el archivo `index.html` con un editor de texto.
2.  Busca el texto que deseas cambiar y reemplázalo por el nuevo.

**Secciones principales a modificar:**

*   **Título y Subtítulo:**
    ```html
    <h1>CONFERENCIA DE ESTACA ALDO BONZI</h1>
    <p class="subtitle">SESIÓN DE ADULTOS</p>
    ```

*   **Autoridades y participantes:**
    ```html
    <div class="info-item"><strong>Preside:</strong> Pte. Alfredo Delgadillo</div>
    <div class="info-item"><strong>Director/a:</strong> Camila Lugo</div>
    <div class="info-item"><strong>Dirige:</strong> Pte. Paul Pizarro</div>
    <div class="info-item"><strong>Pianista:</strong> Elías Savaryn</div>
    ```

*   **Programa (Himnos, Oraciones, Discursantes):**
    Cada parte del programa es un `program-item`. Puedes editar el nombre del participante y su barrio/rama.
    ```html
    <div class="program-item">
        <strong>Oración Inicial:</strong> Agustina Montaño – Bº Villa Madero
    </div>

    <div class="program-item">
        <strong>1º Mensaje:</strong> Matrimonio Ferreira (Asesores Misioneros de Servicio Adultos)
    </div>
    ```
    Para los himnos, puedes cambiar el número y el enlace a la biblioteca de música.
    ```html
    <div class="program-item hymn">
        <strong>Himno Inicial:</strong> <a href="[ENLACE_AL_HIMNO]" target="_blank">#[NÚMERO] "[NOMBRE DEL HIMNO]"</a>
    </div>
    ```

*   **Pie de página (Fecha y Hora):**
    ```html
    <footer>
        <p>Conferencia de Estaca Aldo Bonzi | Sábado 22 de noviembre, 2025 - 18:30 hs</p>
    </footer>
    ```

### 2. Modificar la Apariencia (Estilos)

Si deseas cambiar colores, tamaños de letra o el diseño general, puedes hacerlo en el archivo `css/style.css`.

1.  Abre el archivo `css/style.css` con un editor de texto.
2.  Puedes modificar los valores de las propiedades. Por ejemplo, para cambiar el color de fondo del encabezado:
    ```css
    header {
        background: linear-gradient(180deg, #7dd3fc 0%, #38bdf8 100%); /* Cambia estos colores */
        color: white;
        padding: 40px;
        text-align: center;
    }
    ```

### 3. Cambiar las Imágenes

Las imágenes (logos) se encuentran en la carpeta `images/`. Para cambiarlas:

1.  Consigue las nuevas imágenes que deseas usar.
2.  Asegúrate de que tengan un formato web (como `.png` o `.jpg`).
3.  Reemplaza los archivos en la carpeta `images/` con tus nuevas imágenes. **Es recomendable que los nuevos archivos tengan el mismo nombre** (`logo.png` y `lds-logo.png`) para no tener que modificar el código HTML.

## Visualizar los cambios

Simplemente abre el archivo `index.html` en tu navegador web (Google Chrome, Firefox, etc.) haciendo doble clic sobre él. Cada vez que guardes un cambio en `index.html` o `css/style.css`, recarga la página en el navegador para ver el resultado.
