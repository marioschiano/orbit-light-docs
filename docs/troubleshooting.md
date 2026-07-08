# Risoluzione problemi

## Non vedo l'HDRI nel viewport

Controlla che:

- sei in Material Preview;
- hai cliccato **Create Orbit Light**;
- **Environment Light** è attivo;
- il percorso **HDRI** punta a un file valido;
- **Environment Opacity** non è troppo basso se vuoi vedere anche lo sfondo.

## La scena è troppo scura o troppo chiara

Regola **Environment Exposure (EV)**.

Valori positivi aumentano la luce, valori negativi la riducono.

## Lo sfondo è troppo distratto

Aumenta **Environment Blur** oppure abbassa **Environment Opacity**.

## La rotazione con mouse non funziona

Controlla lo shortcut:

**Shift + Right Mouse Drag**

Se vuoi inclinare verticalmente:

**Shift + Alt + Right Mouse Drag**

## AO Strength o Normal Strength non cambiano nulla

Questi controlli modificano nodi già presenti nel materiale.

Se il materiale non contiene nodi AO/Occlusion o Normal Map compatibili, non ci sarà un cambiamento visibile.

## Le ombre non cambiano

**Shadows Opacity** dipende dai controlli viewport esposti dalla versione di Blender. Se Blender non espone quel valore, lo slider può essere disabilitato.