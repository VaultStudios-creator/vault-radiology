# Installation — vault-radiology

## 1) Prérequis
✅ Obligatoire
- **ox_lib**
- **oxmysql**
- Un système de target :
  - **ox_target** (recommandé) ou **qb-target / qtarget**

✅ Recommandé
- **ox_inventory** (pour l’archive stash + items via exports)

⚠️ Important
- La ressource utilise des **statebags** (rééducation). Assure-toi d’avoir **OneSync** activé (standard sur la plupart des serveurs modernes).

---

## 2) Installation de la ressource
1. Mets le dossier **vault-radiology** dans ton `resources/`
2. Ajoute dans `server.cfg` (ordre conseillé) :

```cfg
ensure oxmysql
ensure ox_lib

# target (au choix)
ensure ox_target
# ou ensure qb-target / ensure qtarget

# inventaire (si utilisé)
ensure ox_inventory

ensure vault-radiology
