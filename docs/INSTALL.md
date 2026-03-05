# Installation — vault-radiology

## Prérequis
- ox_lib
- oxmysql
- Un système target (ox_target / qb-target / qtarget)
- (Recommandé) ox_inventory

## Installation
1) Mets `vault-radiology` dans ton dossier `resources/`
2) Ajoute dans ton `server.cfg` (ordre conseillé) :
```cfg
ensure oxmysql
ensure ox_lib
ensure ox_target
ensure ox_inventory
ensure vault-radiology
