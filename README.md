# ProductDrop.MN — Netlify Deploy Guide

## Folder Structure
```
productdrop/
├── landing.html      ← Public landing page
├── index.html        ← Login + Dashboard  
├── netlify.toml      ← Netlify config
├── _redirects        ← URL routing
└── app/
    ├── beauty.html
    ├── home.html
    ├── health.html
    ├── goods.html
    └── kids.html
```

## Deploy Steps
1. productdrop/ хавтасыг ZIP болгон хадгал
2. netlify.com → "Add new site" → "Deploy manually"
3. ZIP файлаа drag & drop хий
4. Тэрхэнд л URL авна (жишээ: productdrop-mn.netlify.app)

## Custom Domain (productdrop.mn)
1. Netlify → Domain settings → Add custom domain
2. DNS provider дээр: CNAME record → netlify URL руу зааж өг

## Password Change
index.html дотор: `const APP_PASSWORD = "Drop2025#";` гэснийг өөрчил
