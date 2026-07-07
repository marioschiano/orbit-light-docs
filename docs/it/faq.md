# FAQ

## Orbit Light crea una nuova luce nella scena?

Il workflow attuale crea/aggiorna il setup World HDRI. Se esiste una vecchia lampada Orbit Light creata da versioni precedenti, l'addon può rimuoverla.

## Environment Opacity spegne la luce?

No. Environment Opacity cambia la visibilità dello sfondo HDRI, ma l'HDRI continua a illuminare il modello.

## Perché Environment Tilt è disabilitato?

Perché Blender non espone sempre i controlli nativi necessari per inclinare verticalmente la Studio Light. In quel caso Orbit Light mantiene disabilitato lo slider per evitare comportamenti instabili.

## Material Maps modifica tutti i materiali?

Regola nodi AO/Occlusion e Normal Map esistenti quando li trova. Se il materiale non contiene quei nodi, il controllo può non avere effetto visibile.

## Posso importare HDRI personali?

Sì. Usa **Import HDRI Folder** e scegli una cartella con file `.hdr`, `.exr`, `.tx`, `.jpg`, `.jpeg` o `.png`.