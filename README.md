# Calendario Lunar y Astronómico

Esta aplicación web muestra un calendario interactivo que integra las fases lunares y eventos astronómicos importantes. Diseñada con una elegante interfaz en tonos oscuros, ideal para visualizar información astronómica.

## Características

- **Calendario mensual interactivo**: Navegación sencilla entre meses con botones de avance y retroceso
- **Fases lunares**: Muestra la fase lunar para cada día del mes
- **Eventos astronómicos**: Visualiza eventos importantes como eclipses, equinoccios y conjunciones
- **Diseño responsivo**: Adaptable a diferentes tamaños de pantalla
- **Interfaz moderna**: Paleta de colores oscuros ideal para información astronómica

## Tecnologías utilizadas

- HTML5
- CSS3 (con variables CSS para personalización de colores)
- JavaScript (ES6+)
- Diseño orientado a objetos

## Cómo usar

1. Clona este repositorio o descarga los archivos
2. Abre el archivo `index.html` en tu navegador web
3. Navega entre meses utilizando los botones de flecha
4. Observa las fases lunares y eventos astronómicos para cada día

## Personalización

### Colores

Puedes modificar fácilmente la paleta de colores editando las variables CSS en la sección `:root`:

```css
:root {
    --bg-dark: #1a1a2e;     /* Fondo principal */
    --bg-medium: #16213e;   /* Fondo secundario */
    --bg-light: #0f3460;    /* Fondo de elementos interactivos */
    --text-light: #e7e7e7;  /* Color de texto */
    --accent: #4cc9f0;      /* Color de acento para resaltar */
    --moon-color: #f1f1f1;  /* Color para iconos lunares */
    --highlight: #7209b7;   /* Color para resaltar eventos astronómicos */
}
```

### Eventos astronómicos

Puedes agregar o modificar eventos astronómicos editando el objeto `astronomicalEvents` en la clase `LunarCalendar`:

```javascript
this.astronomicalEvents = {
    '2023-3-20': [{ name: 'Equinoccio de Primavera', type: 'event' }],
    '2023-3-25': [{ name: 'Eclipse Lunar', type: 'event' }],
    '2023-3-7': [{ name: 'Conjunción Luna-Marte', type: 'conjunction' }]
};
```

El formato de la fecha es 'AAAA-MM-DD' donde:
- AAAA: año con 4 dígitos
- MM: mes (1-12) 
- DD: día del mes

## Cálculo de fases lunares

El calendario utiliza un algoritmo simplificado basado en un ciclo sinódico lunar de 29.53058867 días, tomando como referencia una luna nueva conocida (7 de marzo de 2023 en la implementación actual).

Para mayor precisión, puedes modificar la fecha de referencia o implementar un algoritmo astronómico más complejo.

## Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue para discutir los cambios importantes antes de realizar un pull request.

## Licencia

Este proyecto está disponible como código abierto bajo la licencia [MIT](https://opensource.org/licenses/MIT).

## Contacto

Si tienes alguna pregunta o sugerencia, no dudes en contactarme a través de mis redes sociales o abriendo un issue en este repositorio.

---

Desarrollado con ❤️ por [Ryu33] con grok3
