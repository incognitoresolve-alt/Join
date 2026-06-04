# BYA-X - Formulaire de Candidature Commerciale

## 🚀 Déploiement Netlify

### 1. Configuration des variables d'environnement

Dans l'interface Netlify (Site settings → Environment variables), ajoutez :

```
GROQ_API_KEY=your_groq_api_key_here
BREVO_API_KEY=your_brevo_api_key_here
```

### 2. Déploiement via GitHub

1. Créez un nouveau repository GitHub
2. Uploadez tous les fichiers de ce ZIP
3. Connectez le repository à Netlify (New site from Git)
4. La configuration est dans `netlify.toml`

### 3. Fichiers importants

| Fichier | Description |
|---------|-------------|
| `index.html` | Formulaire principal (WCAG 2.2 AA + EAA) |
| `accessibilite.html` | Déclaration d'accessibilité obligatoire |
| `netlify/functions/process.js` | Fonction serverless (IA + email) |
| `netlify.toml` | Configuration Netlify (headers sécurité) |

### 4. Conformité légale

- ✅ **EAA** (European Accessibility Act) - Déclaration d'accessibilité
- ✅ **RGPD** - Consentement explicite avec case à cocher
- ✅ **WCAG 2.2 AA** - 25 critères accessibilité vérifiés
- ✅ **EN 301 549 v4.1.1** - Standard européen harmonisé

### 5. Fonctionnalités

- 🎨 Design premium avec glassmorphism
- ♿ Accessibilité complète (skip link, focus management, ARIA)
- 💾 Sauvegarde automatique (localStorage)
- 📊 Indicateur de force du profil en temps réel
- ✅ Dialogue de confirmation avant envoi
- 🔒 Headers sécurité (CSP, HSTS, X-Frame-Options)
- ⏱️ Timeout API (30s) avec AbortController
- 📱 Responsive (mobile-first)

### 6. Tests recommandés

```bash
# Test accessibilité
npm install -g @axe-core/cli
axe http://localhost:8888

# Test contrastes
# Utiliser axe DevTools ou WAVE browser extension
```

---

**Date de mise à jour :** 4 juin 2026
