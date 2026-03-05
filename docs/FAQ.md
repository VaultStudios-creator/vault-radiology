# FAQ — vault-radiology

## Le menu radiologie n’apparaît pas
- Le target est bien démarré (ox_target / qb-target / qtarget)
- Ton job est autorisé (`Config.AllowedJobs`)
- Ton grade est suffisant (`Config.GradePermissions`)
- Les coords sont bonnes (`Config.Radiology.coords`)
Astuce : mets `Config.Radiology.debug = true`

## Problème base de données / rien ne s’enregistre
- `oxmysql` doit démarrer avant `vault-radiology`
- Vérifie ta connexion DB

## Les items ne marchent pas
- Ajoute les items dans ton inventaire
- Copie les images dans le bon dossier (ox_inventory/web/images)
- Si tu as renommé la ressource, adapte les exports (ox_inventory)

## L’archive ne marche pas
L’archive fonctionne surtout avec ox_inventory.
Sinon : désactive `Config.ArchiveStash.enabled`

## Support
Discord : https://discord.gg/vaultstudio
