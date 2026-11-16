# Für das nächste Pack-Update (nach 0.1.9)

- Spieltest 16.11. abends (Screenshots 20:56 in fantasya-0.1.7):
  - [x] Wasser: riesige schwarz-magenta Wand im Meer mit Shader = Earth-Mobs-Pipeline `animation_entity` (vermutl.
    Tropen-Schleim), Iris kannte sie nicht ("Missing program ... in override list"). Fix Fantasya 2d0fde578
    (IrisPipelineCompat meldet sie per Iris-API an) -> braucht neues Fantasya-Jar; im Spiel am Meer gegenpruefen
    (Log muss "Iris: 1 pipeline(s) of ...ANIMATION_ENTITY -> ENTITIES" zeigen, kein "Missing program").
  - [x] Trappermuetze (Waschbaer-Muetze, fantasya:frontier_cap): getragen nur flacher brauner Klotz (Textur
    textures/entity/equipment/humanoid/frontier_cap.png = Kappe ohne Fell/Schwanz), in der Welt mit Shader rosa.
    Hat kein armor2-Mesh -> als armor3-Voxel-Skulptur nachbauen (Fellmuetze + Waschbaerschwanz hinten, Muenze vorn
    wie Item-Icon). Gleiches pruefen fuer emu_leggings, roadrunner_boots, moose_headgear (auch kein armor2-Mesh).
    ERLEDIGT Fantasya e9320a36a (I1 TEIL 0): alle vier als armor3-Skulpturen, im Spiel mit/ohne Shader geprueft
    -> braucht neues Fantasya-Jar.

## Erledigt in 0.1.9 (16.11.)
- PlayerRevive raus (Mod + Config).
- Fantasya 0.1.9 (Morph-Korrekturen, Flug-Sperre für Bewusstlose, JEI-Fundorte mit Biomnamen statt Tag-Pfaden).
- Gefährten 1.0.0 neu im Pack (KI-Begleiter; Ollama optional).
- Spice of Life (Onion): Inventar-Knopf von 130/62 nach 154/-20 (oberhalb des Inventar-Rahmens rechts) - im Spiel ansehen.
