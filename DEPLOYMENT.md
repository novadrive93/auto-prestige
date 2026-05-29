# 🚀 Guide de Déploiement - Auto Prestige

## Option 1: GitHub Pages (Gratuit & Rapide) ⭐

### Étapes:
1. Va dans les **Settings** du repo
2. Scroll vers **GitHub Pages**
3. Sélectionne:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` / `/root`
4. Clique **Save**
5. Attend 1-2 minutes
6. Ton site sera accessible à: `https://novadrive93.github.io/auto-prestige/`

### Avantages:
- ✅ Gratuit
- ✅ HTTPS inclus
- ✅ Déploiement automatique

---

## Option 2: Vercel (Recommandé) ⚡

### Étapes:
1. Va sur [vercel.com](https://vercel.com)
2. Clique **Sign up** et connecte ton GitHub
3. Clique **Add new** → **Project**
4. Sélectionne le repo `auto-prestige`
5. Clique **Deploy**
6. Ton site sera accessible à: `https://auto-prestige.vercel.app/`

### Avantages:
- ✅ Performance maximale (CDN global)
- ✅ Déploiement instantané
- ✅ Domaine personnalisé gratuit
- ✅ Analytics gratuites

---

## Option 3: Netlify (Alternative)

### Étapes:
1. Va sur [netlify.com](https://netlify.com)
2. Clique **Sign up** avec GitHub
3. Clique **Add new site** → **Import an existing project**
4. Sélectionne `novadrive93/auto-prestige`
5. Clique **Deploy site**
6. Ton site sera accessible à: `https://auto-prestige.netlify.app/`

---

## Option 4: Hébergement Classique (OVH, 1&1, etc.)

### Étapes:
1. Clique sur le bouton **<> Code** du repo
2. Clique **Download ZIP**
3. Décompresse le fichier
4. Via FTP, upload `index.html` dans le dossier `public_html` ou `www`
5. Accède à ton domaine

---

## Option 5: Cloudflare Pages

### Étapes:
1. Va sur [pages.cloudflare.com](https://pages.cloudflare.com)
2. Clique **Create a project**
3. Connecte ton GitHub
4. Sélectionne `auto-prestige`
5. Configuration:
   - **Framework preset**: `None`
   - **Build command**: (laisser vide)
   - **Build output directory**: (laisser vide)
6. Clique **Save and Deploy**

### Avantages:
- ✅ CDN ultra-rapide
- ✅ DDoS protection gratuit
- ✅ Email masqué disponible

---

## 🌐 Domaine Personnalisé

### Avec GitHub Pages:
1. Settings → Pages
2. Scroll à "Custom domain"
3. Entre ton domaine (ex: `auto-prestige.fr`)
4. Met à jour les DNS de ton registrar

### DNS Records à ajouter:
```
Type: A
Name: @
Value: 185.199.108.153
```

Répète 3 fois avec:
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

---

## 🔧 Variables d'Environnement (si besoin)

Crée un fichier `.env` (si tu ajoutes du JS backend):
```
WHATSAPP_NUMBER=33600000000
SITE_URL=https://auto-prestige.fr
```

---

## ✅ Checklist Avant Déploiement

- [ ] Vérifie le numéro WhatsApp
- [ ] Teste les liens de navigation
- [ ] Contrôle les images chargent correctement
- [ ] Teste sur mobile (responsive)
- [ ] Vérifie les métadonnées (title, description)
- [ ] Teste les boutons CTA

---

## 📊 Monitoring Post-Déploiement

### Google Analytics:
1. Va sur [google.com/analytics](https://google.com/analytics)
2. Crée un compte
3. Ajoute ce code avant `</head>` dans `index.html`:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Uptime Monitoring:
- [UptimeRobot](https://uptimerobot.com) - Alertes si site down
- [StatusPage.io](https://www.statuspage.io) - Page de statut publique

---

## 🎯 Prochaines Étapes

1. **Ajoute un formulaire de contact** (FormSubmit, Netlify Forms)
2. **Ajoute une base de données** pour gérer les véhicules
3. **Ajoute des images hébergées** localement (pas Unsplash)
4. **Mets en place du SEO** (sitemap.xml, robots.txt)
5. **Ajoute une page Admin** pour mettre à jour l'inventaire

---

**Besoin d'aide? Demande à GitHub Copilot! 🤖**