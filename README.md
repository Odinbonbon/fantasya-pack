# Fantasya Modpack

Minecraft **26.3** mit **NeoForge 26.3.0.99**: Fantasya, Iris + Solas-Shader, Begleit-Mods und **e4mc** zum Zusammenspielen.

## Installieren (Modrinth App oder Prism Launcher)

1. Die neueste `fantasya-x.y.z.mrpack` unter **Releases** herunterladen (rechts auf der Seite).
2. **Modrinth App:** links „+“ → „Aus Datei importieren“ → die `.mrpack` wählen.
   **Prism Launcher:** „Instanz hinzufügen“ → „Importieren“ → die `.mrpack` wählen.
3. Der Launcher lädt alle Mods selbst herunter (Fantasya kommt aus den Releases hier, alles andere von Modrinth).
4. In den Einstellungen der Instanz mindestens **12 GB Arbeitsspeicher** geben. Der erste Start dauert ein paar Minuten.

## Zusammen spielen

- Wer die Welt hat: Welt starten → Esc → **„Für LAN öffnen“** → „LAN-Welt starten“. Im Chat erscheint eine Adresse
  wie `abc-xyz.e4mc.link` (anklicken = kopieren).
- Der andere: Mehrspieler → **Direktverbindung** → Adresse einfügen.
- Beide brauchen **dieselbe Pack-Version**.

## Automatische Updates (einmal einrichten)

Ab Pack 0.1.4 liegt in der Instanz ein kleiner Updater (`fantasya-update.cmd` + `packwiz-installer-bootstrap.jar`).
Einmal in der **Modrinth App** eintragen: Instanz → **Einstellungen** (Zahnrad) → **Launch hooks / Start-Hooks** →
bei **Pre-launch / Vor dem Start** eintragen:

```
cmd /c fantasya-update.cmd
```

Ab dann holt sich die Instanz bei **jedem Start** die neueste Pack-Version von hier (Mods, Configs; ein kleines Fenster
zeigt den Fortschritt). Welten, eigene Einstellungen (`options.txt`) und Tastenbelegungen bleiben erhalten. Ohne Internet
startet das Spiel einfach mit dem alten Stand. Ein neuer Import ist nur noch nötig, wenn sich Minecraft- oder
NeoForge-Version ändern.

Prism Launcher: Instanz bearbeiten → Einstellungen → Eigene Befehle → Vor-Start-Befehl:
`"$INST_JAVA" -jar "$INST_MC_DIR/packwiz-installer-bootstrap.jar" -s client https://raw.githubusercontent.com/Odinbonbon/fantasya-pack/main/pack/pack.toml`

## Updates

Neue Versionen erscheinen hier als neues Release mit einer neuen `.mrpack`. In der Modrinth App bzw. in Prism die
Instanz damit aktualisieren (oder neu importieren; die Welt liegt im Ordner `saves` der Instanz und lässt sich mitnehmen).
