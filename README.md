# Exercice 1 : Système de Paiement Extensible

## 🎯 Objectif
Comprendre le rôle des **interfaces** en Java pour définir des contrats indépendants des implémentations. L'objectif est de découpler le code métier (`PaymentProcessor`) des détails de chaque moyen de paiement (`CreditCard`, `PayPal`, `Bitcoin`) et de pratiquer la gestion dynamique de tableaux.

## 📁 Structure du Projet
- **Package :** `com.example.tp`
- **Classes & Interfaces :**
  - `PaymentMethod.java` : Interface définissant le contrat de paiement (`pay()`, `refund()`, `getName()`).
  - `CreditCard.java` : Implémentation pour la carte bancaire.
  - `PayPal.java` : Implémentation pour la plateforme PayPal.
  - `Bitcoin.java` : Implémentation pour la cryptomonnaie Bitcoin.
  - `PaymentProcessor.java` : Gestionnaire stockant les méthodes de paiement dans un tableau dynamique et traitant les paiements/remboursements.
  - `MainPaiement.java` : Classe de test et d'exécution principale.

## 🛠️ Compilation et Exécution

Depuis le répertoire `src/` :

```bash
javac com/example/tp/*.java
java com.example.tp.MainPaiement
Exercice 2 : `README_EX2.md`

```markdown
# Exercice 2 : Système de Notification Extensible

## 🎯 Objectif
Définir et implémenter une interface Java (`Notification`) pour diffuser des messages via différents canaux (Email, SMS, Push) en appliquant un tri par priorité décroissante via un `Comparator`, le tout piloté par un gestionnaire (`NotificationManager`).

## 📁 Structure du Projet
- **Package :** `com.example.tp`
- **Classes & Interfaces :**
  - `Notification.java` : Interface déclarant `send()`, `getPriority()` et `getType()`.
  - `EmailNotification.java` : Implémentation canal Email (priorité normale = 1).
  - `SMSNotification.java` : Implémentation canal SMS (priorité haute = 2).
  - `PushNotification.java` : Implémentation canal Push (priorité basse = 0).
  - `NotificationManager.java` : Gestionnaire de canaux avec tableau dynamique et tri automatique avant diffusion (`broadcast()`).
  - `MainNotification.java` : Classe de test et d'exécution principale.

## 🛠️ Compilation et Exécution

Depuis le répertoire `src/` :

```bash
javac com/example/tp/*.java
java com.example.tp.MainNotification
```
<img width="1265" height="412" alt="EX2tp8" src="https://github.com/user-attachments/assets/177ce4ef-2724-4ab2-9ee6-0d2fa296782f" />
<img width="1311" height="452" alt="EX1tp8" src="https://github.com/user-attachments/assets/30ef34e4-4cf8-4e40-b643-a2fa13d773f4" />
