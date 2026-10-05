# Guida rapida

## 1. Attiva il lookdev HDRI

1. Apri il modello in Blender.
2. Nel 3D View premi **N** e apri **Orbit Light**.
3. Attiva **Orbit Light ON**.
4. Scegli una HDRI dall'anteprima oppure indica un file nel campo **HDRI**.
5. Lavora in **Material Preview** per vedere materiali PBR, HDRI e blur in tempo reale.

<p align="center">
  <img src="img/placeholder-image.svg" alt="Pannello HDRI Environment" style="max-width:900px;width:100%;">
</p>

Usa **Environment Intensity** per la luce e **Environment Opacity** solo per la visibilità dello sfondo. Portare l'opacità a zero non spegne l'illuminazione HDRI.

## 2. Ruota la luce

Scegli **Drag Target: HDRI**, poi tieni premuto **Shift** e trascina con il **tasto destro** nel 3D View. **Sensitivity** regola la velocità del drag.

Il comando funziona soltanto quando **Orbit Light ON** è attivo.

## 3. Crea uno studio

Apri **Studio Setup**:

1. scegli un **Light Rig Preset**;
2. lascia attivo **Studio Backdrop** e scegli Cyclorama o 360 Dome;
3. lascia attivo **Auto Camera**;
4. premi **Create Studio Setup**.

Puoi modificare intensità e colore di Key, Fill e Rim. **Reset to Preset** ripristina il preset selezionato.

## 4. Salva un'immagine o un turntable

Apri **Turntable**.

- Per un'immagine, imposta cartella, risoluzione, formato Square/16:9 e premi **Capture View**.
- Per controllare il movimento, premi **Start Preview**. Quando la fermi, la rotazione torna al valore iniziale.
- Per il file finale scegli **MP4** o **GIF**, qualità e durata, quindi premi **Create MP4** o **Create GIF**.

Orbit Light mostra separatamente l'avanzamento del rendering dei fotogrammi e quello della creazione del file finale.

## 5. Calibra un materiale

Apri **Calibration** e modifica un parametro. Alla prima modifica Orbit Light crea automaticamente una copia di lavoro e mantiene intatti modello e materiali originali.

Puoi quindi regolare diffuse, roughness, metallic, occlusion, normal ed emission. Per tornare ai valori iniziali usa **Reset Material Calibration**.
