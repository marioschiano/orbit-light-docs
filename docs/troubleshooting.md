# Risoluzione problemi

## Non vedo l'HDRI nel viewport

Controlla che:

- sei in Material Preview;
- hai cliccato **Create Orbit Light**;
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

Controlla anche che **Orbit Light ON** sia attivo e che **Drag Target** sia impostato sul comportamento che vuoi controllare.

## AO Strength o Normal Strength non cambiano nulla

Questi controlli modificano nodi già presenti nel materiale.

Se il materiale non contiene nodi AO/Occlusion o Normal Map compatibili, non ci sarà un cambiamento visibile.

## Le ombre non cambiano

**Shadows** dipende dai controlli viewport esposti dalla versione di Blender. Se Blender non espone quel valore, Orbit Light applica solo i controlli disponibili.
