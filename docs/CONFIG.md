---

## `CONFIG.md`
```md
# Configuration — vault-radiology

Le fichier principal : `shared/config.lua`

## Stack / Détection auto
La ressource peut être en `auto` pour détecter ton framework / inventaire / target.
- Framework : ESX / QBCore / autres (selon ton serveur)
- Inventory : ox_inventory recommandé
- Target : ox_target recommandé

## Jobs & grades
- Autorisations via `Config.AllowedJobs`
- Grades minimum via `Config.GradePermissions` (ex: accès panel, archive, suppression)

## Zone radiologie
Le point radiologie se règle dans :
- `Config.Radiology.coords`
- `Config.Radiology.radius`
- `Config.Radiology.debug` (true pour voir la zone)

## Items utilisés
Radios + rapport + traitements (selon ta config) :
- radios (xray_...)
- rapport (medical_report)
- traitements (attelle/plâtre/chaise roulante/ordonnance/arrêt de travail)

## Options importantes
- Anti-fake (vérif code/token) : `Config.Verify`
- Archive (stash) : `Config.ArchiveStash` (ox_inventory)
- Rééducation / mobilité : `Config.Rehab`
