# Für das nächste Pack-Update (nach 0.1.12)

(noch nichts offen)

## Erledigt in 0.1.12 (19.11.)
- 21.11. nachgeschoben (Client-Ladetest mit allen Pack-Mods gruen): Punchy! Moves, Spatial GUI, Wandering Traveler, Hoverboards, Immersive Panoramas, Jacaranda, Do Another Barrel Roll, Ancient Cities, Animal Garden (Waschbaer, Capybara, Pavian; + Aquarius Libs), Distant Horizons 3.3.4 + Turbo, Ressourcenpaket Fluid & Foolish (nicht voreingestellt aktiv).
- NICHT drin: Diorama 0.11.0 - Client-Absturz nach Teleport ("Texture view Sampler0 horse_white.png has been closed" im GuiRenderer, vermutlich Radar-Gesichter); JourneyMap bleibt deshalb. Nutzerwunsch: JourneyMap raus, sobald Diorama stabil ist.
- Fuer naechste Fantasya-Jar: EndAnimal.isFood null-sicher (End-/Kristalltiere spawnten mit Animal Feeding Trough nicht: "Failed to create mob").
- 21.11. nachgeschoben: Aquaculture 2.11.3 + Baubley Heart Canisters 26.3-1.9.0 (Ladetest Server ok). Powah 9.0.0-alpha NICHT: braucht GuideME 26.3.7 und das NeoForge >= 26.3.0.100 (Pack .99).
- 21.11. nachgeschoben: Gefaehrten 1.2.5 (Vorgabe-Modell gemma3:4b, alte Configs werden einmalig umgestellt; 1.2.4: startet Ollama selbst + laedt fehlendes Modell, stumme Mikrofone werden uebersprungen).
- M-AUFTEILUNG Teil 1: Fantasya Deko als eigene Jar fantasya_deco-1.0.0 (Namensraum fantasya_deco wie vorher,
  Werkbank-Alias fantasya:decor_bench), Fantasya 0.1.12 (Kern ohne Deko). Gefaehrten 1.2.3.

## Erledigt in 0.1.11 (18.11.)
- Fantasya 0.1.11 (NS1 Sternenstahl, NS2 Runenschmied, SP1 Schultertiere, PS1 Pilzsuppen, V2/V3) + Gefaehrten 1.2.0 (G5c, G6d, G7).
- Fallen Knights: config/enderzoology-common.toml (fallen_knight = false) NEU im Pack + Fantasya-Biom-Modifier (Gewicht 3, 1-2).
- Vanilla-Erze gedrosselt (im Jar), Tectonic ocean_offset -0.5 (weniger Meer) - beides nur neue Chunks, in Release-Notiz.
- Corpse raus (Config war nie im Pack). Release-Notiz warnt: vorher Leichen leeren.
- mk_update.py kann jetzt neue Override-Dateien (OVERRIDES_NEU).
- Eribion ist NICHT im Pack -> Daemmerung/Sonnenscheibe (7d88be8) geht nicht mit raus.

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
