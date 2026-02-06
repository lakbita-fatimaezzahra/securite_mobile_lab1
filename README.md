
# securite_mobile_lab1
LAB 1 : Mise en place du lab (Mobexler + snapshot clean)

Étape 1 — Télécharger Mobexler (OVA) et tracer le téléchargement
1 Télécharger l’OVA
  Télécharger depuis le lien officiel (Google Drive) :
  
<img width="1889" height="650" alt="image" src="https://github.com/user-attachments/assets/229b2236-bfae-43f4-b20b-733bf9e53356" />

2 Vérifier l’intégrité (recommandé)
      Si la page officielle fournit un SHA256, calculer le hash local et comparer.
Windows (PowerShell)

Étape 2 — Importer l’OVA dans VirtualBox/VMware
1. VirtualBox → File → Import Appliance
2. Sélectionner .ova → Import
<img width="1416" height="893" alt="image" src="https://github.com/user-attachments/assets/cf25518b-2f87-480f-a94d-33d202900814" />

3. Après import : VM → Settings → Network
Adapter 1 : NAT
<img width="1413" height="360" alt="image" src="https://github.com/user-attachments/assets/56a64555-0deb-4189-8114-156acebcb807" />

Adapter 2 : Host-Only Adapter
<img width="1421" height="491" alt="image" src="https://github.com/user-attachments/assets/a2655937-aa58-4653-9f57-872c3215d5c4" />

Étape 3 — Premier démarrage + connexion

Étape 4 — Vérifier le réseau (tests “santé”)
1 Vérifier IPs
<img width="1912" height="892" alt="image" src="https://github.com/user-attachments/assets/600e0623-6d6a-473e-b0b1-ab60b8bdf552" />
2 Vérifier route par défaut
<img width="1454" height="225" alt="image" src="https://github.com/user-attachments/assets/f5cfb12d-c321-4c3a-9962-f41603dff31e" />
3 Tester Internet
<img width="1457" height="394" alt="image" src="https://github.com/user-attachments/assets/de55706f-6f6d-49fb-94f8-056de7163b03" />
<img width="1680" height="371" alt="image" src="https://github.com/user-attachments/assets/d8caf6f9-176b-4822-9ae2-e22e02498507" />
Étape 5 — Créer le snapshot “CLEAN” (baseline)
VirtualBox
<img width="1919" height="1005" alt="image" src="https://github.com/user-attachments/assets/2af8c980-a3f0-4f1d-b191-71b97c4222f3" />
Étape 6 — Préparer la cible Android (choisir 1 option)
Option B — Émulateur (Genymotion conseillé)
B1. Démarrer un device Genymotion sur l’hôte
B2. Connecter ADB
adb connect <IP_DEVICE>:5555
adb devices




