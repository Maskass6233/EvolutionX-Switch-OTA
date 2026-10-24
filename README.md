<div align="center">

# Evolution X 15.0 — Pixel Tablet Edition
### Pour Nintendo Switch v1 (`nx_tab` / Switchroot)

![Android 15](https://img.shields.io/badge/Android-15.0%20(VanillaIceCream)-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Evolution X](https://img.shields.io/badge/Evolution%20X-v10.6%20Official-0066FF?style=for-the-badge)
![Device](https://img.shields.io/badge/Device-Nintendo%20Switch%20(nx__tab)-E60012?style=for-the-badge&logo=nintendoswitch&logoColor=white)
![Maintainer](https://img.shields.io/badge/Maintainer-Natsuerse-FF6B00?style=for-the-badge)

**Une ROM Android 15 hybride combinant la stabilité matérielle de Switchroot (`ARMv8.0-A`) avec l'interface et les fonctionnalités exclusives de la Google Pixel Tablet (`tangorpro`) sous Evolution X 10.6.**

</div>

---

## 📋 Informations sur la Build

| Propriété | Détail |
| :--- | :--- |
| **Maintainer Officiel** | **Natsuerse** |
| **Appareil cible** | Nintendo Switch v1 (`icosa_tab` / `nx_tab`) |
| **Modèle émulé** | Google Pixel Tablet (`tangorpro` / SKU `GTU8P`) |
| **Version Android** | Android 15 (`BP1A.250505.005` / SDK 35) |
| **Version Evolution X** | `v10.6` (`EvolutionX-10.6-OFFICIAL-by-Natsuerse`) |
| **Architecture CPU** | `ARMv8.0-A` natif (`cortex-a53` / Tegra X1) |
| **Signature OTA** | Certificat privé `RSA-2048` / `SHA-256` (`CN=Natsuerse`) |

---

## ✨ Fonctionnalités Incluses

* 🎨 **Expérience Google Pixel Tablet (`tangorpro`) complète** :
  * **Pixel Launcher** mode Tablette avec barre des tâches persistante et écran partagé fluide.
  * **Hub Mode & Dock Setup** (`DockSetup`) de la Pixel Tablet.
  * **Horloges d'écran de verrouillage Pixel** (`SystemUIClocks-BigNum`, `Calligraphy`, `Flex`, `Growth`, `Inflate`, `Metro`, `Weather`).
  * **Pixel Wallpapers & Styles** (`WallpaperPickerGoogleRelease`).
* ⚡ **Fonctionnalités exclusives Evolution X** :
  * **GameSpace** intégré pour optimiser les performances en jeu sur la Switch.
  * **LMOFreeform** (fenêtres flottantes multi-tâches).
  * Services Google (**GMS**) pré-intégrés et certifiés.
* 🎮 **Support Matériel Nintendo Switch (`nx_tab`) à 100%** :
  * Kernel L4T, GPU NVIDIA Tegra X1, Wi-Fi, Bluetooth, Audio, Dock TV HDMI, capteurs et Joy-Con natifs.
  * Configuration **Tablette Wi-Fi uniquement** (aucun blocage carte SIM dans l'assistant de configuration).
* 🔄 **Mises à jour OTA (Over-The-Air) Directes** :
  * Réception et installation directe des mises à jour depuis **Paramètres → Système → Mises à jour du système** via ce dépôt.
  * Vérification cryptographique stricte : seules les archives signées par la clé privée de **Natsuerse** sont acceptées.

---

## 🚀 Installation (Premier Flash)

1. Démarrez votre Nintendo Switch sur **Hekate** et partitionnez votre carte SD pour Android (minimum **16 Go** recommandés pour Android + stockage interne).
2. Démarrez dans le **Recovery** (LineageOS Recovery / TWRP).
3. Effectuez un **Factory Reset** (*Format Data / Factory Reset*).
4. Allez dans **Apply Update** et flashez :
   * **`EvolutionX-15.0-PixelTablet-nx_tab-Switch.zip`**
   * Puis le patch d'initialisation OTA & Wi-Fi : **`Natsuerse-Maintainer-OTA-SIM-Fix.zip`**
5. Redémarrez (**Reboot System Now**).

---

## 📲 Mises à jour OTA (Over-The-Air)

Vous n'avez plus besoin d'ordinateur ni de reformater votre console pour les mises à jour suivantes :
1. Sur votre Switch, ouvrez **Paramètres → Système → Mises à jour du système**.
2. Appuyez sur **Actualiser** : si une nouvelle version a été publiée par **Natsuerse** dans les [Releases](../../releases) de ce dépôt, elle s'affiche automatiquement.
3. Téléchargez et appuyez sur **Installer** : la Switch vérifie la signature cryptographique `CN=Natsuerse` et installe la mise à jour automatiquement.

---

## 🔐 Sécurité & Signature du Projet

Toutes les builds officielles de ce dépôt sont signées avec le certificat X.509 de **Natsuerse** intégré dans `/system/etc/security/otacerts.zip` :
```text
Subject: C=FR, ST=France, L=Paris, O=Natsuerse Official, OU=EvolutionX Switch Maintainer, CN=Natsuerse
Algorithm: RSA-2048 / SHA256withRSA (Whole-file CMS SignApk)
```

---

## 🙏 Crédits

* **Natsuerse** — *Maintainer du projet, intégration hybride & serveur OTA*
* **Switchroot / LineageOS Team** — *Base matérielle L4T, Kernel & arbres `nx_tab`*
* **Evolution X Team** — *Base Evolution X 15.0 (`tangorpro` v10.6)*
