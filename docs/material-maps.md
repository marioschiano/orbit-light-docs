# Viewport e Calibration

## Viewport Display

**Wireframe Overlay** mostra la topologia sopra ai materiali; quando è attivo compare **Wireframe Opacity**.

**UV Checker** inserisce temporaneamente nodi Texture Coordinate e Checker Texture nello shader esistente, usando la UV attiva. Non crea un nuovo materiale e non sostituisce quello originale. Quando disattivi il controllo, Orbit Light elimina i nodi temporanei e ripristina il collegamento o il colore originale del Base Color.

## Copia di calibrazione automatica

Non serve creare manualmente una copia. Alla prima modifica di un parametro in **Calibration**, Orbit Light duplica automaticamente gli oggetti e i materiali interessati e applica le correzioni alla copia di lavoro. Originali, texture e nodi di partenza restano intatti.

## Substance Painter Match

Questa funzione allinea la lettura PBR tra Substance Painter e Blender:

- **Normal Format**: OpenGL oppure DirectX; con DirectX viene corretto il canale verde.
- **Display Transform**: PBR Neutral, ACES 2.0 oppure Standard sRGB.
- configurazione automatica di sRGB per il colore e Non-Color per mappe dati e packed maps;
- supporto alla lettura di texture packed come ORM, RMA, MRA e MOS;
- impostazioni PBR coerenti per IOR e IOR Level.

Quando disattivi il match, Orbit Light ripristina la precedente gestione colore della scena.

## Controlli di calibrazione

| Gruppo | Controlli |
|---|---|
| **Diffuse / Base Color** | Saturation, Brightness, Contrast e Sharpness. |
| **Roughness** | Brightness, Contrast e Invert per mappe glossiness/smoothness. |
| **Metallic** | Strength, Contrast e Invert. |
| **Surface Detail** | Occlusion Strength, Normal Strength ed Emission Strength. |

**Diffuse Sharpness** campiona pixel vicini nella texture Base Color. Ha effetto sui materiali con Base Color basato su immagine; a zero i nodi temporanei vengono rimossi.

## Bake Missing AO

Se il modello non contiene una mappa di occlusione, scegli **512 px**, **1K**, **2K** o **4K**, imposta **Bake Folder** e premi **Bake Missing AO**. Il bake calcola una self-occlusion dal modello corrente e non richiede una coppia high poly/low poly.

!!! warning "Bake completo"
    Nella versione 1.13.63 il bake della sola AO mancante è operativo. **Bake Calibrated Textures** è ancora disabilitato: il motore che trasferirà tutte le correzioni nelle texture finali è in sviluppo.
