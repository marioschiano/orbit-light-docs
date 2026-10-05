# Riferimento impostazioni

Riferimento dell'interfaccia di Orbit Light **1.13.63**.

## Controllo principale

| Voce | Funzione |
|---|---|
| **Orbit Light ON/OFF** | Decide se Orbit Light intercetta Shift + trascinamento destro e applica i controlli interattivi. |
| **Versione** | Mostra la versione installata in alto a destra. |

## HDRI Environment

| Voce | Valori / funzione |
|---|---|
| **HDRI picker** | Apre la libreria Studio Light di Blender e aggiorna la scena alla selezione. |
| **HDRI** | Percorso del file environment. |
| **Import HDRI Folder** | Importa un'intera cartella nella libreria persistente. |
| **Environment Opacity** | 0-100%; controlla solo la visibilità dello sfondo. Default 100%. |
| **Environment Intensity** | 0-10; controlla la forza luminosa. Default 1.0. |
| **Environment Blur** | 0-100%; blur nativo Material Preview. Default 100%. |
| **Environment Rotation** | Da -360° a 360°; rotazione orizzontale dell'HDRI. |
| **Sensitivity** | Da 0,05 a 2 gradi per pixel di drag. Default 0,35. |
| **Drag Target** | HDRI, Light oppure All Lights. |
| **Shadows** | Sincronizza le ombre di scena/viewport senza spegnere le luci. Default attivo. |

## Viewport Display

| Voce | Funzione |
|---|---|
| **Wireframe Overlay** | Mostra la topologia degli oggetti. |
| **Wireframe Opacity** | Regola l'opacità del wireframe; default 45%. |
| **UV Checker** | Inserisce e rimuove nodi checker temporanei nello shader esistente. |

## Studio Setup

| Voce | Funzione |
|---|---|
| **Light Rig Preset** | Custom più 14 preset fotografici e stilizzati. |
| **Key / Fill / Rim Intensity** | Intensità relativa scalata alle dimensioni del modello. |
| **Key / Fill / Rim Color** | Colore delle tre luci. |
| **Reset to Preset** | Ripristina il preset da cui deriva il rig Custom. |
| **View Lights** | Mostra luci e guide nel viewport; default disattivo. |
| **Studio Backdrop** | Abilita il fondale generato. |
| **Backdrop Shape** | Cyclorama o 360 Dome. |
| **Backdrop** | Sceglie uno dei 12 materiali/colore di fondale. |
| **Backdrop Size** | Scala complessiva del fondale, da 0,5 a 3. |
| **Keep Camera Inside** | Nel Dome limita la camera all'interno della parete. |
| **Backdrop Curve Width** | Ampiezza del raccordo curvo. |
| **Backdrop Curve Sections** | Segmenti della curva, da 2 a 64. |
| **Auto Camera** | Crea una camera frontale inquadrata sul modello. |
| **Keep Camera Aimed at Center** | Mantiene la camera puntata verso un target centrale nascosto. |
| **Create Studio Setup** | Crea o aggiorna rig, fondale e camera. |

## Turntable: Preview e screenshot

| Voce | Valori / funzione |
|---|---|
| **Turntable Speed** | 6-360 gradi al secondo; default 36. |
| **Start/Stop Preview** | Avvia o ferma la rotazione interattiva e poi ripristina l'orientamento. |
| **Output Folder** | Cartella condivisa da screenshot e turntable; default `//orbit_light_captures`. |
| **Screenshot Preset** | 2K, 4K, 1080p oppure UHD. |
| **Screenshot Format** | Square oppure 16:9. |
| **Transparent PNG** | Salva in RGBA ed esclude il fondale generato. |
| **Capture View** | Usa la camera attiva quando presente, altrimenti il viewport. |

## Turntable: MP4 e GIF

| Voce | Valori / funzione |
|---|---|
| **Output Format** | MP4 H.264 oppure GIF in loop. |
| **Video Preset** | Preview 512, 1080p, 2K, 4K. |
| **GIF Resolution** | 512, 768 o 1024 px. |
| **Video Format** | Square oppure 16:9; aggiorna camera e output. |
| **Render Quality** | Fast 16 sample, Balanced 32 sample, High 64 sample Eevee. |
| **Video Duration** | 1-60 secondi per un giro di 360°. |
| **Video FPS** | Valore libero da 1 a 120; preset 24, 30, 60 o Custom. Default 30. |
| **GIF FPS** | 5-24; default 12. |
| **GIF Colors** | 32, 64, 128 o 256. Il formato GIF non può superare 256 colori per fotogramma. |
| **GIF Palette** | Shared (Fast) oppure Per Frame (Best). |
| **Create MP4/GIF** | Avvia rendering JPEG con Eevee e successiva codifica. |
| **Step Progress** | Mostra percentuale, fase, dettagli e tempo. |

## Calibration

| Voce | Valori / funzione |
|---|---|
| **Normal Format** | OpenGL o DirectX per Substance Painter Match. |
| **Display Transform** | PBR Neutral, ACES 2.0 o Standard sRGB. |
| **Diffuse Saturation** | 0-200%; default 100%. |
| **Diffuse Brightness** | Da -100% a 100%; default 0%. |
| **Diffuse Contrast** | Da -100% a 100%; default 0%. |
| **Diffuse Sharpness** | 0-200%; default 0%. Richiede Base Color basato su immagine. |
| **Invert Roughness** | Converte glossiness/smoothness in roughness. |
| **Roughness Brightness/Contrast** | Da -100% a 100%; default 0%. |
| **Metallic Strength** | 0-200%; default 100%. |
| **Metallic Contrast** | Da -100% a 100%; default 0%. |
| **Invert Metallic** | Inverte il canale prima di strength e contrast. |
| **Occlusion Strength** | 0-200%; default 100%. |
| **AO Bake** | 512 px, 1K, 2K o 4K; default 2K. |
| **Bake Folder** | Default `//orbit_light_bakes`. |
| **Normal Strength** | 0-200%; default 100%. |
| **Emission Strength** | 0-500%; default 100%. |
| **Reset Material Calibration** | Ripristina i valori e aggiorna i materiali Working. |

## Funzioni in sviluppo

**Bake Textures** e l'export automatico **FBX / OBJ / GLB** sono disabilitati nella 1.13.63. **Bake Missing AO**, screenshot, MP4 e GIF sono invece operativi.

## Reset Default

Ripristina Studio Softbox, White Studio, Cyclorama, Auto Camera, Keep Camera Aimed at Center, Shadows attive e gli altri valori iniziali dello studio.
