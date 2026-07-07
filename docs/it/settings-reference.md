# Riferimento impostazioni

Questa pagina riassume tutte le voci principali del pannello Orbit Light.

---

## Azioni principali

| Voce | Cosa fa | Quando usarla |
|---|---|---|
| **Create Orbit Light** | Crea o aggiorna il World HDRI, passa allo workspace Shading e imposta Material Preview quando possibile. | Usalo dopo aver scelto una HDRI o quando vuoi aggiornare il setup. |
| **Import HDRI Folder** | Copia una cartella HDRI nella libreria Studio Light di Blender. | Usalo quando vuoi rendere disponibili HDRI personali nel picker nativo. |
| **Rotate Environment** | Avvia la rotazione manuale dell'environment. | Utile se preferisci usare un pulsante invece dello shortcut. |

---

## HDRI Environment

| Voce | Cosa fa | Nota |
|---|---|---|
| **Environment Light** | Abilita la luce HDRI. | Se spento, la forza luminosa viene azzerata. |
| **HDRI** | Immagine environment usata per il World. | Supporta `.hdr`, `.exr`, `.tx`, `.jpg`, `.jpeg`, `.png`. |
| **Environment Opacity** | Controlla la visibilità dello sfondo. | Non spegne l'illuminazione. |
| **Environment Exposure (EV)** | Controlla la forza luminosa. | Valori più alti illuminano di più. |
| **Environment Blur** | Sfoca lo sfondo HDRI in Material Preview. | Usa controlli nativi Blender quando disponibili. |
| **Environment Rotation** | Ruota orizzontalmente l'HDRI. | Può essere controllato anche con Shift + Right Mouse Drag. |
| **Environment Tilt** | Inclina verticalmente l'HDRI. | Disponibile solo se Blender espone il controllo nativo. |
| **Environment Alignment** | Allinea l'HDRI a World o Camera/View. | Utile per diversi workflow di preview. |
| **Sensitivity** | Sensibilità del drag di rotazione. | Aumentala per rotazione più rapida. |

---

## Shadows

| Voce | Cosa fa | Nota |
|---|---|---|
| **Shadows** | Attiva o disattiva le ombre viewport quando disponibili. | Collegato ai controlli Eevee/viewport esposti da Blender. |
| **Shadows Opacity** | Regola l'intensità delle ombre viewport quando supportato. | Lo slider può essere disabilitato se Blender non espone quel valore. |

---

## Material Maps

| Voce | Cosa fa | Nota |
|---|---|---|
| **AO Strength** | Regola nodi AO/Occlusion esistenti. | Non crea AO nuova. |
| **Normal Strength** | Regola nodi Normal Map esistenti. | Non crea normal map nuova. |