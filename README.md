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

## Instrucciones de uso

1. **Abre `cronometro.html`** en un navegador moderno (Chrome, Firefox, Safari, Edge).
2. **Configura tus avisos**, con dos formas de hacerlo:
   - **Calculadora de avisos**: define el tiempo total del examen, los segundos de inicio y cierre, y el número de kata. Presiona "Generar avisos automáticamente" y se crea la lista completa por ti.
   - **Manual**: en la sección "Avisos de tiempo", agrega o edita cada marcador a mano. Puedes trabajar en modo "Por tiempo acumulado" (cada marcador en mm:ss) o "Por duración de cada bloque" (cada marcador en segundos, y si cambias uno, los siguientes se recalculan solos).
3. **Ajusta la cuenta regresiva** (en segundos) que quieres antes de que arranque el cronómetro, y elige si quieres sonido en cada aviso y/o al llegar al tiempo total (el sonido de inicio siempre suena).
4. **Activa la grabación** (opcional): marca la casilla "Grabar con la cámara al iniciar el cronómetro". Al marcarla, el navegador pedirá permiso de cámara — acéptalo. Puedes probarla antes con el botón "Probar cámara".
5. Presiona **"Iniciar cronómetro"** para pasar a la pantalla de examen en pantalla completa.
6. Durante el examen:
   - El botón central inicia, pausa y reanuda el cronómetro.
   - El botón de la izquierda reinicia; si había una grabación en curso, este mismo botón dice **"Finalizar y guardar grabación"** y al presionarlo cierra el video y te da el enlace de descarga.
   - El botón de la derecha activa/desactiva el sonido.
   - Los controles se ocultan solos tras unos segundos en pantalla completa; mueve el mouse, toca la pantalla o presiona una tecla para que vuelvan a aparecer.
7. Para volver a editar los avisos, usa "← Editar avisos" arriba a la izquierda.

### Atajos de teclado (durante el examen)

- **Espacio**: iniciar / pausar
- **R**: reiniciar (y finalizar/guardar la grabación si estaba activa)
- **F**: pantalla completa
- **Esc**: salir de pantalla completa

### ⚠️ Importante para usar la cámara en el celular

Los navegadores móviles bloquean el acceso a la cámara cuando el archivo se abre directamente desde el almacenamiento del teléfono (`file://...`). Para que la grabación funcione en el celular, el archivo debe servirse por **HTTPS** — por ejemplo, publicándolo con GitHub Pages (ver abajo). Abrirlo como archivo local en una computadora de escritorio normalmente sí funciona, pero en Android/iOS no.


# Iaido Exam Timer (English)

A fullscreen timer built to practice and simulate the Iaido exam (shinsa). The clock counts up from 0:00, just like in the real exam, and shows reminders at the moments you define.

## Features

- **Configurable time reminders**: by elapsed time (mm:ss) or by the duration of each block (seconds), with automatic recalculation of the following blocks if you set a total exam time.
- **Reminder calculator**: automatically generates the markers, splitting the time across the number of kata you specify.
- **Distinctive sounds**: a mandatory tone at the start, plus optional sounds on each reminder and when the total time is reached, each with a different pattern so you can tell them apart without looking at the screen.
- **Configurable countdown** before the timer starts.
- **Camera recording**: records video with the clock and current reminder overlaid, at 1080p, so you can review the practice afterward.
- **Bilingual**: Spanish / English, selectable from the page itself.
- **Light / dark theme**, selectable and saved in the browser.
- All your progress (reminders, language, theme) is automatically saved in the browser (`localStorage`) and isn't lost when you close the tab.

## How to use it

1. **Open `cronometro.html`** in a modern browser (Chrome, Firefox, Safari, Edge).
2. **Set up your reminders**, in one of two ways:
   - **Reminder calculator**: set the total exam time, the starting and closing seconds, and the number of kata. Press "Generate reminders automatically" and the full list is created for you.
   - **Manual**: in the "Time reminders" section, add or edit each marker by hand. You can work in "By elapsed time" mode (each marker in mm:ss) or "By duration of each block" mode (each marker in seconds; changing one recalculates the following ones automatically).
3. **Set the countdown** (in seconds) you want before the timer starts, and choose whether you want sound on each reminder and/or when the total time is reached (the start sound always plays).
4. **Turn on recording** (optional): check "Record with the camera when the timer starts". Once checked, the browser will ask for camera permission — allow it. You can test it beforehand with the "Test camera" button.
5. Press **"Start timer"** to move to the fullscreen exam screen.
6. During the exam:
   - The center button starts, pauses, and resumes the timer.
   - The left button resets it; if a recording was in progress, this same button reads **"Finish & save recording"**, and pressing it closes the video and gives you the download link.
   - The right button toggles sound on/off.
   - The controls auto-hide after a few seconds in fullscreen; move the mouse, tap the screen, or press a key to bring them back.
7. To go back and edit the reminders, use "← Edit reminders" in the top-left corner.

### Keyboard shortcuts (during the exam)

- **Space**: start / pause
- **R**: reset (and finish/save the recording if one was in progress)
- **F**: fullscreen
- **Esc**: exit fullscreen

### ⚠️ Important for using the camera on mobile

Mobile browsers block camera access when the file is opened directly from the phone's storage (`file://...`). For recording to work on mobile, the file needs to be served over **HTTPS** — for example, by publishing it with GitHub Pages (see below). Opening it as a local file on a desktop computer usually works fine, but not on Android/iOS.

