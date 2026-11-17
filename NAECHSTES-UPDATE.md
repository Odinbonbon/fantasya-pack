# Für das nächste Pack-Update (nach 0.1.10)

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
