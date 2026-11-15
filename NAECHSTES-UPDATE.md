# Für das nächste Pack-Update (nach 0.1.8)

- **PlayerRevive raus** (Nutzer 15.11. ~19:55: "player revive fliegt aus der Liste beim nächsten Update").
  `pack/mods/PlayerRevive_NEOFORGE_v2.1.3_mc26.3.pw.toml` löschen, `packwiz refresh`, Config
  `config/playerrevive*.json` mit entfernen. Grund: Bewusstlos-Zustand ("bleeding out") nach Tod/Verhungern, setzt das
  Essen herunter; als gedownter Vogel konnte man noch fliegen (in Fantasya jetzt ohnehin gesperrt: MorphService.downed).
- Fantasya-Jar mit den Morph-Animations-Korrekturen (Rabe/Krähe/Elster, Ghoul, Ossukage, Hase, ...) und der Flug-Sperre
  für Bewusstlose/Tote mitliefern.
