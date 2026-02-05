# 🎣 Site de Réservation - Section Carpe de Soufflenheim

## 📋 Description
Site web de réservation en ligne pour les week-ends libre de pêche à l'étang Landgraben.

### Fonctionnalités
✅ Carte interactive de l'étang avec 10 postes de pêche  
✅ Réservation en ligne avec paiement PayPal  
✅ Gestion de 4 sessions annuelles  
✅ Interface admin pour gérer les dates et réservations  
✅ Postes déplaçables pour ajuster leur position  
✅ Système de disponibilité en temps réel avec **Supabase**  
✅ Synchronisation automatique entre tous les utilisateurs

---

## 🎉 NOUVEAU : Migration vers Supabase

Votre site utilise maintenant **Supabase** au lieu de Firebase !

### ✅ Ce qui est déjà configuré :
- Base de données Supabase connectée
- Synchronisation temps réel activée
- Toutes les fonctionnalités opérationnelles

### 🔑 Vos identifiants Supabase :
- **URL** : `https://drhsdlzhxkbamwcskblr.supabase.co`
- **Table** : `sessions`
- Les clés sont déjà intégrées dans les fichiers HTML

---

## 🚀 Déploiement sur Netlify

### Étapes :

1. **Préparer les fichiers** :
   - Tous vos fichiers sont prêts : `index.html`, `admin.html`, `config.json`, `pond.jpg`, `logo.png`

2. **Déployer sur Netlify** :
   - Allez sur [netlify.com](https://netlify.com)
   - "Add new site" → "Deploy manually"
   - Glissez-déposez TOUS les fichiers
   - C'est en ligne ! 🎉

3. **Tester** :
   - Visitez votre site
   - Testez une réservation (elle sera enregistrée dans Supabase)
   - Vérifiez l'admin (mot de passe : `Souffcarpe1664`)

---

## 📍 Positionner les postes

1. **Admin** → Mot de passe : `Souffcarpe1664`
2. **"📍 Modifier les positions des postes"**
3. **Glissez-déposez** les postes
4. **"💾 Enregistrer"** → Télécharge `config.json`
5. **Re-déployer** sur Netlify avec le nouveau fichier

---

## 🔧 Configuration

### Mot de passe admin
`Souffcarpe1664`

### PayPal
Dans `index.html` ligne ~626, changez :
```javascript
window.location.href = 'https://www.paypal.me/votrecompte/30EUR';
```

### Dates des sessions
Via l'admin → Modifier directement

---

## 📱 Utilisation

**Visiteurs :**
1. Choisir session (◄ ►)
2. Cliquer sur poste vert
3. Remplir formulaire
4. Payer PayPal

**Admin :**
1. Bouton "⚙️ Admin"
2. Mot de passe
3. Gérer les sessions, dates, réservations

---

## 🔄 Structure de la base Supabase

Votre table `sessions` contient :
- `id` : ID auto (clé primaire)
- `session_id` : 1, 2, 3 ou 4
- `date` : Texte (ex: "15-16 Mars 2025")
- `reservations` : JSON (liste des réservations)
- `closed_spots` : JSON (postes fermés manuellement)
- `created_at` : Timestamp

Tout est synchronisé automatiquement ! 🚀

---

## 🆘 Besoin d'aide ?

Contactez-moi pour :
- Configuration PayPal  
- Ajout de fonctionnalités
- Support technique

---

## ✅ Avantages de Supabase vs Firebase

✅ Pas de problème d'`eval()` avec Netlify  
✅ Synchronisation temps réel native  
✅ Base PostgreSQL robuste  
✅ Interface admin claire  
✅ Gratuit jusqu'à 500 MB de stockage
