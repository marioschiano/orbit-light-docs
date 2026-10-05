# Shortcut e rotazione

## Shift + tasto destro

Nel 3D View tieni premuto **Shift** e trascina con il **tasto destro del mouse**.

Il risultato dipende da **Drag Target**:

- **HDRI** ruota orizzontalmente l'environment.
- **Light** orbita una singola Orbit Light attorno al centro del modello.
- **All Lights** ruota insieme Key, Fill e Rim dello Studio Setup; il movimento verticale controlla anche l'inclinazione del rig.

## Quando il comando è attivo

Lo shortcut è intercettato soltanto con **Orbit Light ON**. Se Orbit Light è disattivato, Shift + tasto destro mantiene il comportamento normale di Blender.

**Sensitivity** cambia la risposta del trascinamento. Un valore basso consente regolazioni fini; un valore alto rende la rotazione più rapida.

## Centro dell'orbita

Orbit Light calcola il centro dal modello e ignora gli oggetti generati dallo studio. Il target della camera e quello delle luci sono protetti e nascosti per evitare spostamenti accidentali.

!!! tip
    Per regolare una singola luce scegli **Light**. Per conservare i rapporti del preset e ruotare l'intero set scegli **All Lights**.
