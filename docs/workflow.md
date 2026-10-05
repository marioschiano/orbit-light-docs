# Workflow operativo

Le sezioni principali sono indipendenti: puoi usare soltanto l'HDRI, creare uno studio, produrre un turntable oppure calibrare i materiali. Non è necessario completarle in sequenza.

## HDRI e viewport

Attiva **Orbit Light ON**, scegli l'HDRI e regola visibilità, luce, blur e rotazione. In **Viewport Display** puoi sovrapporre il wireframe o attivare un checker UV temporaneo.

## Studio Setup

Apri la tendina **Studio Setup** per creare un set coerente con le dimensioni del modello.

### Light Rig

I preset disponibili sono:

**Studio Softbox, Product, High Key, Beauty, Rembrandt, Split, Hard Surface, Top Light, Rim Focus, Sunset, Night, Neon, Comic e Horror**, oltre a **Custom**.

Per ogni preset puoi modificare intensità e colore di **Key**, **Fill** e **Rim**. La prima modifica passa a Custom senza alterare il preset di origine. **Reset to Preset** ripristina i suoi valori originali.

**View Lights** mostra o nasconde nel viewport luci e guide, senza cambiare l'illuminazione.

### Fondale

**Studio Backdrop** crea uno dei due fondali:

- **Cyclorama**: fondale fotografico frontale, largo e profondo, con raccordo regolabile.
- **360 Dome**: fondale circolare per muovere la camera attorno all'oggetto senza scoprire il vuoto.

I preset includono White Studio, Warm White, Light Grey, Grey Clay, Warm Grey, Cool Grey, Dark Studio, Infinite Black, Midnight Blue, Burgundy, Chroma Green e Chroma Blue.

Con il Dome, **Keep Camera Inside** limita la distanza della camera in base alle dimensioni del fondale. Se cambi **Backdrop Size**, il limite si aggiorna insieme al Dome.

### Camera

**Auto Camera** crea e inquadra la camera sul modello. **Keep Camera Aimed at Center** usa un target nascosto e un vincolo per mantenere la camera orientata verso il centro. Dopo la creazione, Camera to View è attivo per consentire di rifinire l'inquadratura navigando nel riquadro camera.

Premi **Create Studio Setup** per creare o aggiornare il set. Il pulsante cestino rimuove gli elementi generati.

## Turntable

### Preview

**Start Preview** ruota il modello nel viewport alla velocità indicata in gradi al secondo. **Stop Preview** ferma il movimento e ripristina la rotazione iniziale.

### Still Capture

**Capture View** salva un PNG. Se esiste una camera attiva usa quella e renderizza con Eevee; senza camera cattura il viewport corrente. Il formato Square/16:9 aggiorna subito l'aspect ratio della camera.

Con **Transparent PNG** il fondale generato viene escluso dalla cattura, senza cancellarlo dalla scena.

### MP4 e GIF

La creazione del turntable avviene in due fasi:

1. **Rendering Frames**: Eevee renderizza dalla camera una sequenza JPEG qualità 92 usando la GPU.
2. **Encoding**: i fotogrammi diventano un MP4 H.264 o una GIF.

Ogni fase ha una percentuale da 0 a 100, dettaglio del fotogramma corrente e tempo trascorso. Il rendering non apre a tutto schermo la finestra Render Result e può essere annullato dal pulsante accanto a Create.

Velocità e durata sono collegate: un giro completo è sempre 360°, quindi aumentando **Turntable Speed** diminuisce automaticamente **Video Duration**, e viceversa.

## Calibration

Alla prima regolazione Orbit Light crea automaticamente una copia di lavoro. L'utente continua a lavorare sul modello visibile, mentre l'originale rimane intatto.

Usa **Substance Painter Match** per allineare normal map, color space e display transform, poi calibra i canali. **Bake Missing AO** è già disponibile. Il bake completo delle texture calibrate è indicato nel pannello come funzione futura.

## Export

La sezione Export rappresenta il modello finale previsto per FBX, OBJ e GLB. Nella versione 1.13.63 l'esportazione automatica non è ancora implementata; usa gli exporter nativi di Blender seguendo i [consigli export](export-tips.md).

## Reset Default

Il pulsante in fondo al pannello ripristina i valori di studio predefiniti, compresa la spunta **Shadows** attiva.
