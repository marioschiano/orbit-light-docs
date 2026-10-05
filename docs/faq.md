# FAQ

## Orbit Light usa una lampada per l'HDRI?

No. L'illuminazione ambientale deriva da una texture HDRI nel World. Le luci Key, Fill e Rim appartengono invece allo **Studio Setup** e sono opzionali.

## Opacity a zero spegne la luce?

No. **Environment Opacity** nasconde lo sfondo, ma l'HDRI continua a illuminare e a comparire nei riflessi. Per ridurre la luce usa **Environment Intensity**.

## Perché Shift + tasto destro non fa sempre la stessa cosa?

Il comportamento dipende da **Drag Target**: HDRI, Light oppure All Lights. Inoltre lo shortcut è attivo soltanto con **Orbit Light ON**.

## Posso modificare un preset di luci?

Sì. Tutti i preset mostrano intensità e colore di Key, Fill e Rim. Alla prima modifica il rig passa a **Custom**; **Reset to Preset** ripristina il preset di origine.

## UV Checker sostituisce il materiale?

No. Inserisce nodi temporanei nello shader già esistente e ripristina il Base Color quando lo disattivi.

## Calibration modifica l'originale?

No. Alla prima regolazione viene creata automaticamente una copia Working. Mesh, materiali, texture e nodi originali restano intatti.

## Posso convertire una glossiness in roughness?

Sì. Attiva **Invert Roughness**. È utile anche quando una smoothness/glossiness arriva da un canale alpha packed.

## Posso creare AO senza un modello high poly?

Sì. **Bake Missing AO** calcola la self-occlusion direttamente dal modello corrente.

## Una GIF può avere più di 256 colori?

Il formato GIF classico usa al massimo 256 colori per singolo fotogramma. **Per Frame (Best)** genera una palette adattiva per ogni frame: non supera il limite del formato, ma mantiene meglio le variazioni cromatiche rispetto a una palette condivisa.

## Dove vengono salvati screenshot e turntable?

Nella cartella **Output Folder**. Il valore predefinito è `//orbit_light_captures`, relativo al file `.blend`. Se il progetto non è ancora salvato, Orbit Light usa `Documenti/orbit_light_captures` e, se necessario, la cartella temporanea di Blender.

## Bake ed export sono completi?

Nella 1.13.63 sono operativi **Bake Missing AO**, Capture, MP4 e GIF. Il bake completo delle texture calibrate e l'export automatico FBX/OBJ/GLB sono ancora in sviluppo.
