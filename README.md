# Newsletter "Interview Déclic Sportifs"

Template de newsletter premium pour accompagner la reconversion des sportifs professionnels.

## 📁 Fichiers

| Fichier | Description |
|---------|-------------|
| `newsletter-declic-sportifs.html` | Template principal avec variables à remplacer |
| `preview-exemple.html` | Version preview avec contenu d'exemple |
| `variante-vert-foret.html` | Variante avec couleur accent vert forêt |

## 🎨 Palette de couleurs

**Version principale (Bleu profond)**
- Fond : `#f7f7f7` (gris très clair) / `#ffffff` (blanc)
- Texte principal : `#1a1a1a` (anthracite)
- Accent : `#1a365d` (bleu profond)
- Texte secondaire : `#555555`, `#888888`

## 📝 Variables à remplacer

Toutes les variables sont au format `{{NOM_VARIABLE}}` pour une compatibilité maximale avec Brevo, Mailjet, SendinBlue, etc.

### Contenu principal

| Variable | Description | Exemple |
|----------|-------------|---------|
| `{{PREHEADER_TEXT}}` | Texte aperçu email (non visible) | "Marie Dupont raconte son déclic..." |
| `{{MOIS_ANNEE}}` | Mois et année de l'édition | "Janvier 2026" |
| `{{ACCROCHE_LIGNE_1}}` | Première ligne du titre hero | "Quand la carrière s'arrête," |
| `{{ACCROCHE_LIGNE_2}}` | Deuxième ligne (en couleur accent) | "personne ne t'explique quoi faire après." |
| `{{INTRO_TEXTE}}` | Texte d'introduction (3-4 lignes) | "Ce mois-ci, une ancienne..." |

### Portrait de l'invité

| Variable | Description | Exemple |
|----------|-------------|---------|
| `{{PORTRAIT_IMAGE_URL}}` | URL de la photo portrait | "https://..." |
| `{{INVITE_NOM}}` | Prénom + Nom | "Marie Dupont" |
| `{{INVITE_SPORT}}` | Sport + précision | "Handball · Équipe de France" |
| `{{INVITE_STATUT}}` | Statut actuel | "Retraitée depuis 2024" |

### Contenu éditorial

| Variable | Description |
|----------|-------------|
| `{{MOMENT_CLE_TITRE}}` | Titre de la section moment clé |
| `{{MOMENT_CLE_PARAGRAPHE_1}}` | Premier paragraphe |
| `{{MOMENT_CLE_PARAGRAPHE_2}}` | Deuxième paragraphe |
| `{{CITATION_TEXTE}}` | Citation forte de l'invité |
| `{{PROJECTION_TITRE}}` | Titre section projection |
| `{{PROJECTION_TEXTE}}` | Texte adressé au lecteur |

### Call to Action

| Variable | Description | Exemple |
|----------|-------------|---------|
| `{{CTA_URL}}` | Lien du bouton | "https://..." |
| `{{CTA_TEXTE}}` | Texte du bouton | "Découvrir l'interview complète" |
| `{{CTA_SOUS_TEXTE}}` | Sous-texte optionnel | "Lecture de 8 minutes" |

### Footer & Signature

| Variable | Description |
|----------|-------------|
| `{{SIGNATURE_MESSAGE}}` | Message personnel |
| `{{SIGNATURE_NOM}}` | Prénom de l'expéditeur |
| `{{SIGNATURE_ROLE}}` | Rôle/fonction |
| `{{UNSUBSCRIBE_URL}}` | Lien de désinscription |
| `{{PRIVACY_URL}}` | Lien politique de confidentialité |
| `{{ANNEE}}` | Année en cours |
| `{{NOM_SOCIETE}}` | Nom de la société |

## 📱 Responsive

Le template est **mobile-first** avec des breakpoints à 600px :
- Textes adaptés pour mobile
- Image portrait centrée sur mobile
- Bouton CTA pleine largeur sur mobile
- Padding réduit sur les côtés

## 🔧 Intégration

### Brevo (ex-SendinBlue)
1. Créer une nouvelle campagne email
2. Choisir "Importer un template HTML"
3. Coller le code HTML
4. Remplacer les variables par les variables dynamiques Brevo `{{ contact.FIELD }}`

### Mailjet
1. Template Builder > Import HTML
2. Coller le code
3. Utiliser les variables Mailjet `[[var:VARIABLE]]`

### Mailchimp
1. Créer une campagne > Code your own
2. Coller le HTML
3. Utiliser les merge tags `*|VARIABLE|*`

## ✅ Bonnes pratiques

- **Images** : Utiliser des images optimisées (< 200KB), hébergées sur un CDN
- **Portrait** : Idéalement 360x440px, format JPG, noir & blanc
- **Alt text** : Toujours renseigner les attributs alt des images
- **Test** : Tester sur Litmus ou Email on Acid avant envoi

## 🚫 À éviter

- Ajouter des boutons supplémentaires
- Utiliser des GIFs ou animations
- Surcharger de couleurs
- Mettre des liens dans la citation
