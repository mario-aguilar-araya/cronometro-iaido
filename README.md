# Cronómetro de examen de Iaido

Cronómetro de pantalla completa pensado para practicar y simular el examen de Iaido (shinsa). El tiempo sube desde 0:00, como en el examen real, y va mostrando avisos en los momentos que tú definas.

## Características

- **Avisos de tiempo configurables**: por tiempo acumulado (mm:ss) o por duración de cada bloque (segundos), con recálculo automático de los bloques siguientes si defines un tiempo total de examen.
- **Calculadora de avisos**: genera automáticamente los marcadores repartiendo el tiempo entre el número de katas que indiques.
- **Sonidos distintivos**: un tono obligatorio al iniciar y sonidos opcionales en cada aviso y al llegar al tiempo total, cada uno con un patrón distinto para reconocerlos sin mirar la pantalla.
- **Cuenta regresiva configurable** antes de que arranque el cronómetro.
- **Grabación con cámara**: graba video con el reloj y el aviso actual superpuestos, en 1080p, para revisar la práctica después.
- **Bilingüe**: español / inglés, seleccionable desde la propia página.
- **Paleta clara / oscura**, seleccionable y guardada en el navegador.
- Todo el progreso (avisos, idioma, tema) se guarda automáticamente en el navegador (`localStorage`), no se pierde al cerrar la pestaña.

## Uso

Es un archivo HTML único (`cronometro.html`), sin dependencias externas. Basta con abrirlo en un navegador moderno (Chrome, Firefox, Safari, Edge).

### ⚠️ Importante para usar la cámara en el celular

Los navegadores móviles bloquean el acceso a la cámara cuando el archivo se abre directamente desde el almacenamiento del teléfono (`file://...`). Para que la grabación funcione en el celular, el archivo debe servirse por **HTTPS** — por ejemplo, publicándolo con GitHub Pages (ver abajo). Abrirlo como archivo local en una computadora de escritorio normalmente sí funciona, pero en Android/iOS no.
