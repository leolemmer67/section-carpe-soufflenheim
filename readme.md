# 🎣 Site de Réservation - Section Carpe de Soufflenheim

## 📋 Description
Site web de réservation en ligne pour les week-ends libre de pêche à l'étang Landgraben.

### Fonctionnalités
✅ Carte interactive de l'étang avec 10 postes de pêche  
✅ Réservation en ligne avec paiement PayPal  
✅ Gestion de 4 sessions annuelles  
✅ Interface admin pour gérer les dates et réservations  
✅ Postes déplaçables pour ajuster leur position  
✅ Système de disponibilité en temps réel  
✅ **Positions synchronisées** pour tous les visiteurs

---

## 🚀 Comment mettre en ligne (GRATUIT)

### Netlify (Recommandé)

1. **Créer un compte gratuit** sur [netlify.com](https://netlify.com)

2. **Préparer les fichiers** :
   - Créer un dossier "site-peche"
   - Y mettre : `index.html`, `admin.html`, `config.json`, `README.md`
   - Y mettre vos images : `pond.jpg` (étang) et `logo.png` (logo)

3. **Déployer** :
   - Netlify → "Add new site" → "Deploy manually"
   - Glisser-déposer tout le dossier
   - C'est en ligne ! 🎉

4. **Connecter votre domaine** :
   - "Domain settings" → "Add custom domain"
   - Suivre les instructions DNS

---

## 📍 Positionner les postes (IMPORTANT)

### Comment ça marche maintenant

Les positions sont **centralisées** dans `config.json` :
- ✅ Tous les visiteurs voient la même chose (PC, mobile, tablette)
- ✅ Une seule fois à configurer
- ✅ Facile à mettre à jour

### Étapes pour positionner les postes

1. **Sur votre PC** → Allez sur votre site
2. **Admin** → Mot de passe : `Souffcarpe1664`
3. **"📍 Modifier les positions des postes"**
4. **Glissez-déposez** les 10 postes au bon endroit
5. **"💾 Enregistrer"** → Le fichier `config.json` se télécharge 📥
6. **Sur Netlify** → "Deploys" → Glissez le dossier complet avec le nouveau `config.json`
7. **Fini !** Tout le monde voit les bonnes positions ✅

---

## 🔧 Configuration

### Mot de passe admin
**Souffcarpe1664**

### PayPal (ligne ~380 dans index.html)
```javascript
window.location.href = 'https://www.paypal.me/votrecompte/30EUR';
```

### Dates des sessions
Via l'admin → Modifier directement

### Fermer des postes
Admin → Grille des postes → 🔒 Fermer / 🔓 Rouvrir

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
3. Gérer tout !

---

## 🆘 Besoin d'aide ?

Contactez-moi pour :
- Déploiement
- Configuration PayPal  
- Ajout de fonctionnalités
- Migration vers base de données

---

## 🔄 Mise à jour des positions

**Important :** Chaque fois que vous déplacez les postes :
1. Mode édition → Déplacer → Sauvegarder
2. **Télécharger** le nouveau `config.json`
3. **Redéployer** sur Netlify avec ce fichier

Sinon les positions ne seront pas synchronisées ! ⚠️