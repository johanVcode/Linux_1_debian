# Linux 1 - Projekt: Mediaserver Baseline & Hardening

Detta repository fungerar som dokumentation och logg för min lärare under min hardening-fas i Linux 1-kursen. Det visar systemets ursprungliga grundinställningar innan vidare konfiguration.

## Systemöversikt (Nuvarande Baseline)
- **Operativsystem:** Debian Trixie (Minimal headless-installation i grunden)
- **Nuvarande skrivbordsmiljö:** GNOME (Används temporärt under den första konfigurationsfasen)
- **Brandvägg:** `ufw` är installerat för att säkra systemet (Aktiveras efter att portar har verifierats)

## Implementerad loggning för kursen
1. **Konfigurationshantering (`etckeeper` + `git`):** Initierat i mappen `/etc` för att automatiskt versionshantera och logga varenda ändring som görs i systemets filer.
2. **Automatiskt ändringsregister (`system_changes.log`):** Alla framtida paketinstallationer och rader som ändras i systemfilerna exporteras automatiskt från `etckeeper` till detta repository.
