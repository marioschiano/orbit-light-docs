# Risoluzione problemi

## Non vedo l'HDRI

- Attiva **Orbit Light ON**.
- Passa a **Material Preview**.
- Verifica che il file HDRI esista o scegli un'immagine dal picker.
- Aumenta **Environment Opacity** se vuoi vedere anche lo sfondo.

Se il modello è illuminato ma lo sfondo non è visibile, l'opacità può essere a zero: è un comportamento previsto.

## Intensity, blur o rotation non cambiano la scena

Controlla di essere in Material Preview e di non avere **Scene World** attivo nelle opzioni Viewport Shading. Se usi il campo HDRI, verifica che il percorso sia valido. Cambia temporaneamente **Environment Intensity** a un valore molto diverso per confermare l'aggiornamento.

## La rotazione del mouse non parte

1. attiva **Orbit Light ON**;
2. porta il cursore nel 3D View;
3. verifica **Drag Target**;
4. usa Shift + trascinamento con tasto destro, non un semplice clic.

Con Orbit Light OFF lo shortcut viene lasciato a Blender.

## Disattivando Shadows cambiano anche le luci

Nella 1.13.63 la spunta deve disattivare soltanto le ombre. Premi **Reset to Preset** per riallineare il rig, poi aggiorna lo Studio Setup. Se il problema continua, indica preset e versione Blender nel bug report.

## Il cyclorama o il Dome lasciano vedere il vuoto

Aumenta **Backdrop Size** e aggiorna lo Studio Setup. Con il 360 Dome lascia attivo **Keep Camera Inside**. Il limite segue le dimensioni del Dome, ma non impedisce di modificare manualmente la focale o il clipping della camera.

## La camera non guarda il centro

Attiva **Keep Camera Aimed at Center** e premi nuovamente **Create Studio Setup**. Orbit Light ricrea il target centrale nascosto e il vincolo della camera.

## Lo screenshot o il video hanno un'inquadratura diversa

- Verifica che **Orbit Light Camera** sia la camera attiva della scena.
- Scegli Square o 16:9 prima di rifinire l'inquadratura.
- Entra in Camera View e usa Camera to View per la regolazione finale.
- Non cambiare aspect ratio dopo aver composto l'immagine senza ricontrollare il frame.

## Il render copre l'interfaccia

Orbit Light imposta il display del render su `NONE` durante Capture e turntable. Se Blender continua ad aprire Render Result, controlla di usare la 1.13.63 e riavvia Blender dopo l'aggiornamento.

## Blender sembra fermo durante il turntable

Controlla **Step Progress**:

- Step 1/2 renderizza i fotogrammi con Eevee;
- Step 2/2 crea MP4 o GIF.

Full HD, 2K, 4K, qualità High, 60 FPS e GIF Per Frame aumentano sensibilmente il tempo. Per un test usa Preview 512, Balanced e 30 FPS.

## La GIF è nera o ha colori molto diversi

Usa **Per Frame (Best)** e 256 colori. Verifica prima che un singolo **Capture View** abbia colori corretti. Alcuni visualizzatori gestiscono male profili e palette GIF: confronta il file anche in un browser moderno.

## Non trovo i file creati

Controlla **Output Folder**. Con il valore predefinito e un `.blend` salvato, la cartella `orbit_light_captures` si trova accanto al progetto. Con un file non salvato viene usata la cartella Documenti dell'utente.

## Un controllo Calibration non ha effetto

- Diffuse Sharpness richiede un'immagine collegata al Base Color.
- Normal Strength richiede un nodo Normal Map compatibile.
- Occlusion Strength agisce sui nodi AO/Occlusion trovati o sulla AO generata.
- Le correzioni sono applicate alla copia Working, non al materiale originale.
