# Inspection e controlli materiale

La sezione **Inspection** aiuta a controllare rapidamente materiali, UV, wireframe e normal map senza uscire dal workflow principale di Orbit Light.

<p align="center">
  <img src="img/placeholder-image.svg" alt="Inspection in Orbit Light" style="max-width:900px;width:100%;">
</p>

---

## Inspection Mode

**Inspection Mode** permette di passare tra tre viste:

- **Original** mantiene i materiali originali.
- **Clay** applica una vista neutra per leggere forme, volumi e shading.
- **UV Checker** applica una texture checker temporanea per controllare stretching e distribuzione UV.

## Wireframe Overlay

**Wireframe Overlay** mostra la topologia sopra al modello.

Quando è attivo, **Wireframe Opacity** controlla quanto il wireframe appare visibile.

## Normal Check

**Normal Check** applica un preset di controllo utile per individuare shading rotto, normal map troppo deboli o problemi di lettura della superficie.

## AO Strength

Regola input di forza su nodi o gruppi AO/Occlusion quando sono già presenti nel materiale.

Non crea automaticamente una mappa AO nuova.

## Normal Strength

Regola la forza dei nodi **Normal Map** già presenti nel materiale.

Non crea automaticamente una normal map nuova.

!!! note "Importante"
    AO Strength e Normal Strength lavorano sui nodi esistenti. Se il materiale non contiene AO/Occlusion o Normal Map collegati, il controllo potrebbe non produrre cambiamenti visibili.
