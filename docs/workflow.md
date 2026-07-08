# Workflow manuale

Orbit Light combina illuminazione HDRI, controllo materiali, pipeline PBR, capture e turntable in un unico pannello.

---

## 1. Crea l'environment

Scegli una HDRI nel pannello **HDRI Environment** e clicca **Create Orbit Light**.

Orbit Light crea o aggiorna il World HDRI, passa allo workspace Shading e imposta il 3D View in Material Preview quando possibile.

<p align="center">
  <img src="img/placeholder-image.svg" alt="Create Orbit Light workflow" style="max-width:900px;width:100%;">
</p>

---

## 2. Controlla luce, viewport e materiali

Usa **Environment Opacity**, **Environment Exposure (EV)**, **Environment Blur** ed **Environment Rotation** per regolare la luce e lo sfondo.

Usa **Shift + Right Mouse Drag** per ruotare l'HDRI direttamente nel viewport. Durante la rotazione Orbit Light mostra un HUD temporaneo, così puoi vedere il valore mentre lavori.

La sezione **Inspection** serve per controllare il modello:

- **Inspection Mode** passa tra Original, Clay e UV Checker.
- **Wireframe Overlay** mostra la topologia sopra al modello.
- **Normal Check** applica una vista utile per controllare problemi di normali.
- **AO Strength** e **Normal Strength** regolano i nodi già presenti nei materiali.

---

## 3. Usa la PBR Pipeline

La sezione **PBR Pipeline** è divisa in tre step.

### STEP 1 Calibration

Premi **Create Calibration Copy** per creare una copia di lavoro non distruttiva.

Qui puoi regolare:

- **Hide Original**
- **Base Saturation**
- **Base Brightness**
- **Base Contrast**
- **Roughness Brightness**
- **Roughness Contrast**
- **Metallic Strength**
- **Emission Strength**

Usa **Reset Material Calibration** per riportare i valori di calibrazione ai default.

### STEP 2 Bake

La sezione **STEP 2 Bake** prepara il bake delle texture calibrate.

Nella versione attuale il pulsante **Bake Textures** è presente come step di pipeline, ma il bake engine è indicato come funzione in arrivo.

### STEP 3 Export

La sezione **STEP 3 Export** prepara una copia export del modello.

Il pulsante **Prepare Export Model** crea una copia dedicata all'export. L'esportazione FBX / OBJ / GLB è indicata come funzione in arrivo.

---

## 4. Studio Setup

Usa **Studio Setup** quando vuoi creare rapidamente una scena da presentazione:

- **Light Rig Preset** sceglie il mood della luce.
- **Create Backdrop** abilita il cyclorama.
- **Backdrop** sceglie il tipo di fondale.
- **Backdrop Radius Scale** regola la scala del fondale.
- **Backdrop Bevel Segments** controlla la morbidezza della curva.
- **Create Camera** aggiunge una camera inquadrata sul modello.
- **Create Studio Setup** genera rig, backdrop e camera.
- Il pulsante con cestino rimuove lo studio setup generato.

---

## 5. Capture e Turntable

La sezione **Capture** salva screenshot dal viewport o dalla camera.

Imposta **Output Folder**, **Screenshot Preset**, **Screenshot Format** e **Transparent PNG**, poi clicca **Capture View**.

La sezione **Turntable** crea anteprime e video 360:

- **Turntable Speed** controlla la velocità della preview nel viewport.
- **Start Preview** avvia la rotazione del modello.
- **Stop Preview** ferma la preview.
- **Video Preset**, **Video Format**, **Video Duration** e **FPS** controllano il video.
- **Render Turntable MP4** genera un video turntable.

---

## 6. Asset Info

La sezione **Asset Info** mostra un riepilogo tecnico del modello selezionato:

- Objects
- Vertices
- Triangles
- Materials
- UV Maps
- Textures

Premi **Refresh Asset Info** per aggiornare i dati.
