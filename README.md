# BâtiPro (MAB) - Application de Gestion pour Entrepreneurs du Bâtiment

**BâtiPro** est une application Flutter multi-plateforme (Android, iOS, Windows, macOS, Linux), **100% hors-ligne (Offline-first)** conçue pour les artisans et entrepreneurs du bâtiment (maçons, plombiers, électriciens, peintres, carreleurs, menuisiers et entreprises générales).

---

## 🏗️ Noms d'application recommandés

1. **BâtiPro** *(Recommandé)* : Moderne, percutant, inspire la rigueur professionnelle et résonne parfaitement en français et à l'international.
2. **MAB BâtiPro** : Conserve le nom de code du projet *(Métiers & Artisans du Bâtiment)* comme signature de marque.
3. **ChantierPro** / **باتي برو** : Nom bilingue idéal pour le déploiement sur les marchés francophones et arabophones (Maghreb, Moyen-Orient).

---

## 🚀 Fonctionnalités Implémentées

### 1. 🧰 Modèles par Métier au Premier Lancement
- **Maçonnerie & Gros Œuvre** : Ciment CPJ 45, Sable (m³), Gravier (m³), Fer à béton Ø12 / Ø8, Briques creuses, Parpaings, Planches de coffrage.
- **Plomberie & Chauffage** : Tubes PVC, Multicouche, Raccords, Vannes d'arrêt, Mitigeurs, Colle PVC, Téflon.
- **Électricité & Domotique** : Câbles H07V-U 1.5mm² / 2.5mm², Disjoncteurs 16A / 20A, Gaines ICTA, Prises, Interrupteurs, Spots LED.
- **Peinture & Finitions** : Peinture blanche sous-couche, Satinée, Enduit de lissage, Rouleaux anti-goutte, Ruban de masquage.
- **Carrelage & Revêtements** : Mortier-colle, Joints hydrofuges, Grès cérame 60x60, Croisillons autonivelants.
- **Entreprise Générale / Tous Corps d'État** : Catalogue mixte prêt à l'emploi.
- *Possibilité de modifier, ajouter ou réinitialiser le catalogue à tout moment depuis les Paramètres.*

### 2. 🏛️ Gestion Complète des Chantiers
- Création et suivi de chantiers (Client, Adresse/Localisation, Budget, Dates, Statuts : *En cours, En attente, Terminé, Annulé*).
- **Vue 360° du chantier** :
  - Consommation budgétaire en temps réel avec jauge de progression.
  - Onglet **Stock & Matériaux consommés** sur le chantier.
  - Onglet **Ouvriers & Pointages** affectés avec coût de la main d'œuvre.
  - Onglet **Frais directs & Caisse** (carburant, outillage, location de matériel).
  - Calcul automatique du **Bénéfice estimé**.
  - **Génération instantanée du Rapport de Chantier en PDF**.

### 3. 📦 Stock & Alertes de Réapprovisionnement
- Gestion des articles avec unités adaptées (*Sac, m³, m², kg, pièce, rouleau, pot 15L...*).
- **Alerte visuelle "Stock bas"** dès qu'un article passe sous son seuil de sécurité.
- **Entrées de stock** (Achats fournisseurs avec prix unitaire).
- **Sorties de stock** (Affectation directe et décompte sur un chantier précis).
- Historique complet des mouvements et valorisation totale du stock.

### 4. 👷 Employés, Pointage Journalier & Paie Automatisée
- Fiche ouvrier : Nom, Téléphone, Rôle, Salaire journalier ou mensuel.
- **Feuille de pointage rapide du jour** :
  - Statuts : *Présent (1j)*, *Demi-journée (0.5j)*, *Absent*.
  - Saisie rapide des heures supplémentaires.
  - Affectation en un clic de l'équipe entière à un chantier.
- **Gestion des acomptes / avances sur salaire**.
- **Calcul automatique de la paie** :
  $$\text{Net à payer} = (\text{Jours travaillés} \times \text{Tarif}) + (\text{Heures sup} \times \text{Taux}) - \text{Acomptes versés}$$

### 5. 👥 Contacts Clients & Fournisseurs (CRM)
- Carnet d'adresses dédié au BTP avec solde restant / dettes.
- **Appel téléphonique en 1 clic** (`tel:`).
- **Lien direct WhatsApp en 1 clic** avec message prérempli (`wa.me`).

### 6. 📄 Devis & Factures avec Génération PDF & Partage
- Création de Devis et Factures avec numérotation automatique.
- Lignes de prestations & matériaux dynamiques (Désignation, Unité, Qté, P.U., Total).
- Gestion de la TVA, des remises, acomptes déjà réglés et reste à payer.
- **Aperçu PDF en direct** avec mise en page soignée, logo BâtiPro et coordonnées de l'artisan.
- **Partage PDF instantané** via WhatsApp, email ou impression.

### 7. 💰 Dépenses & Caisse
- Saisie des frais directs de chantier et de caisse (Carburant, Location de matériel, Outillage, Restauration, Transport).
- Suivi analytique par catégorie.

### 8. 📊 Tableau de Bord & Rapports
- Indicateurs clés : Chantiers actifs, Dépenses globales, CA encaissé, Valeur stock, Trésorerie nette.
- Alertes critiques et raccourcis d'actions rapides.

### 9. 🌐 Bilingue Français & Arabe (RTL Support)
- Support natif du Français et de l'Arabe avec inversion dynamique de la direction d'écriture (RTL).
- Changement de langue instantané depuis l'en-tête de l'application.

---

## 🛠️ Stack Technique

- **Framework** : Flutter 3.47+ / Dart 3.13+
- **Gestion d'état** : Riverpod (`AsyncNotifierProvider` / `NotifierProvider`)
- **Base de données** : SQLite local avec `sqflite` et `sqflite_common_ffi` (Desktop & Mobile)
- **PDF & Impression** : `pdf` et `printing`
- **Communications** : `url_launcher` (Appels et WhatsApp)
- **Préférences** : `shared_preferences`

---

## 💻 Lancement

```bash
# Récupération des dépendances
flutter pub get

# Lancement des tests
flutter test

# Exécution de l'application (Windows, Android, iOS, etc.)
flutter run
```
