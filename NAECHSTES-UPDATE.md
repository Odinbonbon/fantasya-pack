# Für das nächste Pack-Update (nach 0.1.10)

- Fallen Knights (Ender Zoology) VIEL SELTENER (Nutzer 17.11. ~22:30): Mod spawnt sie mit 1/4 Zombie-Gewicht in Gruppen 4-6
  ueberall in der Oberwelt. Loesung = ZUSAMMEN ausliefern: (1) NEUE Pack-Datei config/enderzoology-common.toml (bisher nicht
  im Pack, Vorlage = Nutzer-Instanz, dort schon `fallen_knight = false`) mit `fallen_knight = false` -> mk_update.py braucht
  dafuer "Override neu anlegen"; (2) Fantasya-Jar mit data/fantasya/neoforge/biome_modifier/compat_enderzoology_fallen_knight.json
  (fantasya 3da8f5ffc: Gewicht 3, 1-2 Stueck, nur wenn Ender Zoology geladen; Reittier kommt von selbst) = ~25x seltener.
  Nur (1) ohne (2) = gar keine Ritter. Im Spiel ueber mehrere Naechte pruefen.
- Vanilla-Erze gedrosselt (V3 f, Nutzer "zu haeufig"): steckt im Fantasya-Jar (data/minecraft/worldgen/placed_feature/ore_*),
  gilt nur fuer NEUE Chunks. Je Chunk mit Pack-Weltgen: Diamant 24 -> 12, Redstone 35 -> 25, Lapis 22 -> 15, Gold 25 -> 19;
  Eisen/Kohle/Kupfer unveraendert. In der Release-Notiz erwaehnen (alte Welt behaelt ihre schon erzeugten Erze).
- WENIGER MEER (Fantasya V3 a, Nutzer "weniger Meer"): pack/config/tectonic.json ocean_offset -0.8 -> -0.5 (schon im Repo
  geaendert) -> Meer 52 % -> 34 %, Tiefsee bleibt (11 %). mk_update.py braucht dafuer OVERRIDES_TEXT fuer
  overrides/config/tectonic.json (Zeile `"ocean_offset": -0.8,` -> `-0.5,`). Gilt nur fuer NEUE Chunks: in alten Welten
  Stufen an der Grenze erkundet/neu -> Release-Notiz "fuer neue Welten" (Nutzer-Frage in fantasya/docs/nutzer-urteil.md V3 a).
- Corpse-Mod RAUS (Nutzer 17.11. ~22:20): pack/mods/corpse-*.pw.toml + Config corpse* entfernen (in mk_update.py RAUS =
  ["mods/corpse-"], OVERRIDES_RAUS = ["overrides/config/corpse"]). VORHER WARNEN: Gegenstaende in noch liegenden Leichen
  gehen verloren -> vor dem Update alle Leichen leeren. Danach fallen Sachen beim Tod wieder normal auf den Boden
  (verschwinden nach 5 min). Ladetest ohne Corpse (haengt ein anderer Mod davon ab? Pruefung wie bei VeinMiner).

## Erledigt in 0.1.10 (17.11.)
- Fantasya 0.1.10: Iris-Wasserfix (Earth-Mobs-Pipeline), Trappermuetze/Elch/Emu/Laufvogel als armor3, Mantel-Absturz-Fix,
  W1 TerraBlender-Regionen (terrablender.toml region_size 5, vanilla weight 4), U1 eigener Ultimine.
- Gefaehrten 1.1.0: Stimme + Push-to-Talk (V) + Dienst-Autostart. Offen fuers oeffentliche Pack: Einrichtungsanleitung
  Stimmen-Dienst (Python, Piper-Minimalpaket), Vorgabe `daten`; xtts/damien NIE ins Pack.
- VeinMiner (+ Config) raus. KotlinLangForge BLEIBT: Fzzy Config ist Kotlin (tomlkt, keine Kotlin-Stdlib im Jar) und
  Subtle Effects braucht Fzzy Config.
- options.txt bobView:false (Kopfwippen aus; wirkt nur bei neuen Instanzen, options.txt ist preserve).
- Ladetest: alle 183 Instanz-Mods + Fantasya 0.1.10 im Gefaehrten-Dev-Client, Welt + ferne Chunks, kein Absturz.

## Erledigt in 0.1.9 (16.11.)
- PlayerRevive raus (Mod + Config).
- Fantasya 0.1.9 (Morph-Korrekturen, Flug-Sperre für Bewusstlose, JEI-Fundorte mit Biomnamen statt Tag-Pfaden).
- Gefährten 1.0.0 neu im Pack (KI-Begleiter; Ollama optional).
- Spice of Life (Onion): Inventar-Knopf von 130/62 nach 154/-20 (oberhalb des Inventar-Rahmens rechts) - im Spiel ansehen.
- Fantasya e46f2b88e (17.11. Nacht): Server-Absturz beim Tragen des Alchemistenmantels (kupfer_cloak) mit Solonion behoben -> neue Fantasya-Version ins Pack.
- Eribion 7d88be8 (18.11.): Daemmerung heller (ownDusk 10, ownDuskGi 4,5) + weisse Sonnenscheibe. Wer die Regler Daemmerungslicht/Daemmerung indirekt einmal verstellt hat, behaelt seinen Wert (eribion.properties) - im Changelog erwaehnen.
