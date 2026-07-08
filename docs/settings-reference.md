# Riferimento impostazioni

Questa pagina riassume le voci principali dell'attuale pannello Orbit Light.

---

## Controlli principali

| Voce | Cosa fa | Quando usarla |
|---|---|---|
| **Orbit Light ON / OFF** | Abilita o disabilita i controlli viewport di Orbit Light. | Usalo quando vuoi spegnere temporaneamente il setup senza rimuovere la scena. |
| **Create Orbit Light** | Crea o aggiorna il World HDRI, passa allo workspace Shading e imposta Material Preview quando possibile. | Usalo dopo aver scelto una HDRI o quando vuoi aggiornare il setup. |

---

## HDRI Environment

| Voce | Cosa fa | Nota |
|---|---|---|
| **HDRI picker** | Usa il picker nativo Material Preview / Studio Light di Blender. | Utile per scegliere rapidamente un ambiente già disponibile. |
| **HDRI** | Immagine environment usata per il World. | Supporta `.hdr`, `.exr`, `.tx`, `.jpg`, `.jpeg`, `.png`. |
| **Import HDRI Folder** | Copia una cartella HDRI nella libreria Studio Light di Blender. | Le HDRI restano disponibili anche dopo il riavvio di Blender. |
| **Environment Opacity** | Controlla la visibilità dello sfondo. | Non spegne l'illuminazione. |
| **Environment Exposure (EV)** | Controlla la forza luminosa. | Valori più alti illuminano di più. |
| **Environment Blur** | Sfoca lo sfondo HDRI in Material Preview. | Usa controlli nativi Blender quando disponibili. |
| **Environment Rotation** | Ruota orizzontalmente l'HDRI. | Può essere controllato anche con Shift + Right Mouse Drag. |
| **Sensitivity** | Sensibilità del drag di rotazione. | Aumentala per una rotazione più rapida. |
| **Rotate Environment** | Avvia la rotazione manuale dell'environment. | È il pulsante con icona mouse vicino a Sensitivity. |
| **Drag Target** | Decide cosa controlla il drag interattivo. | Utile quando vuoi separare rotazione environment e comportamento viewport. |
| **Environment Shadows** | Attiva le ombre dell'environment quando Blender le espone. | Dipende dai controlli viewport disponibili nella versione di Blender. |

---

## Inspection

| Voce | Cosa fa | Nota |
|---|---|---|
| **Inspection Mode - Original** | Mostra i materiali originali. | È la modalità normale di lavoro. |
| **Inspection Mode - Clay** | Applica una visualizzazione clay temporanea. | Utile per leggere forme, volumi e shading senza texture. |
| **Inspection Mode - UV Checker** | Applica una visualizzazione checker temporanea. | Utile per controllare stretching e leggibilità UV. |
| **Wireframe Overlay** | Mostra la topologia sopra al modello. | Aiuta a controllare densità e struttura della mesh. |
| **Wireframe Opacity** | Regola la trasparenza del wireframe. | Appare quando Wireframe Overlay è attivo. |
| **Normal Check** | Applica un preset di controllo per le normali. | Utile quando vuoi individuare shading rotto o normali invertite. |
| **AO Strength** | Regola nodi AO/Occlusion esistenti. | Non crea AO nuova. |
| **Normal Strength** | Regola nodi Normal Map esistenti. | Non crea normal map nuova. |

---

## PBR Pipeline

| Voce | Cosa fa | Nota |
|---|---|---|
| **Pipeline Status** | Mostra lo stato della pipeline. | Si aggiorna dopo le operazioni principali. |
| **STEP 1 Calibration** | Apre lo step per creare una copia di lavoro e calibrare i materiali. | È lo step più operativo della pipeline attuale. |
| **STEP 2 Bake** | Mostra lo step dedicato al bake. | Il bake engine è indicato come funzione in arrivo. |
| **STEP 3 Export** | Mostra lo step dedicato all'export. | FBX / OBJ / GLB export è indicato come funzione in arrivo. |

### STEP 1 Calibration

| Voce | Cosa fa | Nota |
|---|---|---|
| **Hide Original** | Nasconde il modello originale dopo la creazione della copia di calibrazione. | Mantiene il workflow non distruttivo. |
| **Create Calibration Copy** | Crea una copia di lavoro per calibrare materiali e preparare il modello. | Non modifica direttamente l'originale. |
| **Base Saturation** | Regola la saturazione del base color. | Lavora sulla copia/materiali di calibrazione. |
| **Base Brightness** | Regola la luminosità del base color. | Utile per uniformare texture troppo scure o chiare. |
| **Base Contrast** | Regola il contrasto del base color. | Utile per rendere più leggibile il materiale. |
| **Roughness Brightness** | Regola la luminosità della roughness. | Influenza il comportamento visivo delle superfici. |
| **Roughness Contrast** | Regola il contrasto della roughness. | Utile per separare aree più o meno lucide. |
| **Metallic Strength** | Regola il contributo metallic. | Utile per materiali PBR con metallic map o valori metallic. |
| **Emission Strength** | Regola il contributo emission. | Utile per materiali con emissione già presente. |
| **Reset Material Calibration** | Riporta i valori di calibrazione ai default. | È il pulsante con icona reset/loop. |

### STEP 2 Bake

| Voce | Cosa fa | Nota |
|---|---|---|
| **Bake Textures** | Rappresenta lo step di bake delle texture calibrate. | Nella versione attuale è disabilitato e mostra "Bake engine coming next.". |

### STEP 3 Export

| Voce | Cosa fa | Nota |
|---|---|---|
| **Prepare Export Model** | Crea una copia dedicata all'export. | Lo step segnala che FBX / OBJ / GLB export arriverà in una versione futura. |

---

## Studio Setup

| Voce | Cosa fa | Nota |
|---|---|---|
| **Light Rig Preset** | Sceglie il preset di illuminazione studio. | Include Studio Softbox, Product, Sunset, Night, Comic e Horror. |
| **Create Backdrop** | Abilita la creazione del fondale/cyclorama. | Se attivo mostra i controlli Backdrop. |
| **Backdrop** | Sceglie il tipo di fondale. | Include White Studio, Grey Clay, Dark Studio e Infinite Black. |
| **Backdrop Radius Scale** | Regola la scala del fondale rispetto al modello. | Utile per modelli molto piccoli o molto grandi. |
| **Backdrop Bevel Segments** | Controlla la morbidezza della curva del fondale. | Valori più alti rendono il fondale più morbido. |
| **Create Camera** | Crea una camera inquadrata sul modello. | Utile per screenshot e turntable. |
| **Create Studio Setup** | Genera rig luci, camera e backdrop. | Usa i valori impostati nella sezione. |
| **Remove Studio Setup** | Rimuove lo studio setup generato. | È il pulsante con icona cestino. |

---

## Capture

| Voce | Cosa fa | Nota |
|---|---|---|
| **Output Folder** | Cartella dove salvare screenshot e video. | Di default usa `//orbit_light_captures`. |
| **Screenshot Preset** | Sceglie la risoluzione dello screenshot. | Include 2K, 4K, 1080p e UHD. |
| **Screenshot Format** | Sceglie formato Square o 16:9. | Influenza risoluzione X/Y del render. |
| **Transparent PNG** | Salva PNG con trasparenza quando possibile. | Può nascondere il backdrop durante la cattura. |
| **Capture View** | Salva uno screenshot dalla camera o dal viewport. | Usa la camera se lo studio setup l'ha creata e impostata. |
| **Progress** | Mostra avanzamento dell'operazione di capture. | Appare durante operazioni attive. |

---

## Turntable

| Voce | Cosa fa | Nota |
|---|---|---|
| **Turntable Speed** | Controlla la velocità della preview nel viewport. | Valore in gradi al secondo. |
| **Start Preview** | Avvia la rotazione del modello nel viewport. | Non esporta un video, serve per preview interattiva. |
| **Stop Preview** | Ferma la preview turntable. | Appare quando la preview è in corso. |
| **Video Preset** | Sceglie la risoluzione del video. | Include Preview 512, 1080p, 2K e 4K. |
| **Video Format** | Sceglie Square o 16:9. | Influenza il formato finale. |
| **Video Duration** | Durata del giro 360. | Valore in secondi. |
| **FPS** | Fotogrammi al secondo. | Valori più alti sono più fluidi ma più lenti da renderizzare. |
| **Render Turntable MP4** | Crea un video MP4 turntable non distruttivo. | Usa Eevee/OpenGL e salva nella cartella Output Folder. |

---

## Asset Info

| Voce | Cosa fa | Nota |
|---|---|---|
| **Refresh Asset Info** | Aggiorna le statistiche del modello. | Usalo dopo aver cambiato selezione o scena. |
| **Objects** | Numero di oggetti rilevati. | Dato informativo. |
| **Vertices** | Numero di vertici. | Dato informativo. |
| **Triangles** | Numero di triangoli. | Dato informativo. |
| **Materials** | Numero di materiali. | Dato informativo. |
| **UV Maps** | Numero di UV maps. | Dato informativo. |
| **Textures** | Numero di texture rilevate. | Dato informativo. |

---

## Preferences

| Voce | Cosa fa | Nota |
|---|---|---|
| **Check for Updates** | Controlla il manifest online di Orbit Light. | Segnala se esiste una versione più recente. |
| **Open Documentation** | Apre la documentazione online. | Al momento apre la versione italiana alla root del sito. |
| **Release Notes** | Apre il changelog online. | Usa il link del manifest se disponibile. |
| **Video Tutorials** | Apre il canale YouTube. | Punta al canale Mario Schiano 3D. |
