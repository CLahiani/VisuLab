# VisuLab

Interface web de conception de scénarios de démonstration (Veeam) : éditeur graphique de topologies (machines, hyperviseurs, zones, liens), stockage des scénarios en fichiers JSON, et génération des livrables de provisioning.

## Utilisation

Ouvrir `visulab.html` dans Chrome ou Edge (aucune installation, fichier unique).

- **Bibliothèque** : glisser-déposer des composants Veeam (VBR, Proxy, Repository…), hyperviseurs (ESXi, Hyper-V, Proxmox VE), infrastructure (VM, Kubernetes, Container, Database, S3 immuable…), zones (Zone, Datacenter, Salle) et formes.
- **Liens** : tirer depuis la pastille verte d'un objet vers un autre.
- **Propriétés** : nom, IP, rôle, OS, description, couleurs (panneau de droite).
- **Sélection multiple** : cadre à la souris ou Shift+clic, puis alignement/répartition.
- **Scénarios** : bouton 📁 pour choisir le dossier de travail ; enregistrement direct en JSON (`Ctrl+S`), historique dans la colonne de gauche, import/export.
- **Présentation** : mode plein écran lecture seule (🎬), mode confidentialité (👁).
- **Exports** : image PNG/SVG, et 🚀 Provisioning → script bash KVM/libvirt (cloud-init) ou runbook Markdown détaillé.

## Structure

- `visulab.html` — l'application complète (HTML/CSS/JS, sans dépendance)

Les scénarios sont enregistrés en JSON dans le dossier de travail choisi via le bouton 📁 — ils restent locaux et ne sont pas versionnés dans ce dépôt.
