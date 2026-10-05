# Consigli export

L'export automatico FBX/OBJ/GLB è ancora in sviluppo nella versione 1.13.63. Nel frattempo puoi esportare con gli strumenti nativi di Blender.

## Prima di esportare

1. Conserva il modello originale come riferimento.
2. Verifica scala, trasformazioni, normali e UV.
3. Controlla il materiale con **Substance Painter Match** e l'environment desiderato.
4. Ricorda che le correzioni Calibration sono nodi di lavoro: finché il bake completo non sarà disponibile, non diventano automaticamente nuove texture.
5. Usa **Bake Missing AO** soltanto quando ti serve una mappa AO ricavata dalla mesh corrente.

## Unity e Unreal

La corrispondenza visiva dipende anche da shader, color management, normal format e packing del motore di destinazione.

- Unity usa spesso smoothness/glossiness nell'alpha di una texture packed.
- Unreal usa comunemente ORM: Occlusion, Roughness e Metallic nei canali RGB.
- Imposta le texture dati come Non-Color e il Base Color come sRGB.
- Verifica sempre normal OpenGL/DirectX e l'eventuale inversione del canale verde.

!!! note
    Il futuro workflow Bake/Export di Orbit Light è progettato per creare un modello finale semplificato e texture calibrate/packed. Non è ancora disponibile nella 1.13.63.
