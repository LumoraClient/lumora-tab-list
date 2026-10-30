# Lumora Tab-Liste & Scoreboard

Ping als Zahl in Millisekunden in der Tab-Liste; Scoreboard verschieben, skalieren, ohne Zahlen anzeigen oder ausblenden.

Eingebautes Addon des Lumora Clients (Id `lumora-tab`, im Spiel: Lumora-Hub → Addons). Läuft in allen 18
unterstützten Minecraft-Versionen (1.8.9 bis 26.3). Standard: **an**.

> Dieses Repository ist eine **Kopie zum Lesen und Nachschlagen**. Das Addon ist Teil des Clients, weil es an
> Minecraft-Stellen andockt, die sich je Version unterscheiden. Gebaut, getestet und ausgeliefert wird es in
> [LumoraClient/lumora-launcher](https://github.com/LumoraClient/lumora-launcher). Eigene Addons baust du mit dem
> [Addon-Template](https://github.com/LumoraClient/lumora-addon-template).

## Einstellungen

| Schlüssel | Bedeutung |
|---|---|
| `ping_numbers` | Ping als Zahl in der Tab-Liste |
| `scoreboard` | Scoreboard anzeigen |
| `scoreboard_scale` | Scoreboard-Größe (%) |
| `scoreboard_x` | Scoreboard nach links |
| `scoreboard_y` | Scoreboard nach oben/unten |
| `hide_numbers` | Rote Zahlen ausblenden (ab 1.20.4) |

## Aufbau

| Ordner | Inhalt | Im Haupt-Repository |
|---|---|---|
| `src/` | Das Addon (versionsunabhängig, nur Lumora-API und Lumora-Core) und die gemeinsamen Helfer, die es braucht | `lumora-core/src/main/java/dev/lumora/core/` |
| `hooks/<version>/` | Die Andockstellen je Minecraft-Version (Mixins und Adapter) | `client/mc<version>/src/main/java/dev/lumora/client/` |
| `tests/` | Unit-Tests (laufen im Haupt-Repository) | `lumora-core/src/test/java/` |

## Lizenz

GPL-3.0-or-later (siehe `LICENSE`), wie der ganze Lumora Client.
