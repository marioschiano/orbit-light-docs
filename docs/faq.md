# FAQ

## Orbit Light crea una nuova luce nella scena?

Il workflow attuale crea/aggiorna il setup World HDRI. Se esiste una vecchia lampada Orbit Light creata da versioni precedenti, l'addon può rimuoverla.

## Environment Opacity spegne la luce?

No. Environment Opacity cambia la visibilità dello sfondo HDRI, ma l'HDRI continua a illuminare il modello.

## Dove controllo UV, wireframe e normal map?

Usa la sezione **Inspection**.

Da lì puoi passare tra **Original**, **Clay** e **UV Checker**, attivare **Wireframe Overlay**, usare **Normal Check** e regolare **AO Strength** o **Normal Strength** quando il materiale contiene già nodi compatibili.

## AO Strength e Normal Strength modificano tutti i materiali?

Regola nodi AO/Occlusion e Normal Map esistenti quando li trova. Se il materiale non contiene quei nodi, il controllo può non avere effetto visibile.

## Posso importare HDRI personali?

Sì. Usa **Import HDRI Folder** e scegli una cartella con file `.hdr`, `.exr`, `.tx`, `.jpg`, `.jpeg` o `.png`.
