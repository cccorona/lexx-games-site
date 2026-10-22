# Publicar este sitio (repo público)

JalapeoMerge es **privado** → no sirve para GitHub Pages de tienda.

## 1. Crear repo vacío en GitHub

1. Abre https://github.com/new
2. Name: `lexx-games-site`
3. **Public**
4. **Sin** README / .gitignore / license (vacío)
5. Create repository

## 2. Push desde esta carpeta

En la máquina local (desde la raíz de JalapeoMerge):

```bash
GITDIR="$(pwd)/.git-lexx-games-site"
WORKDIR="$(pwd)/lexx-games-site"
git --git-dir="$GITDIR" --work-tree="$WORKDIR" push -u origin main
```

Si aún no existe el remote:

```bash
git --git-dir="$GITDIR" --work-tree="$WORKDIR" remote add origin https://github.com/cccorona/lexx-games-site.git
git --git-dir="$GITDIR" --work-tree="$WORKDIR" push -u origin main
```

## 3. Activar Pages

Repo `lexx-games-site` → Settings → Pages → Deploy from branch **main** / **root**.

URL: https://cccorona.github.io/lexx-games-site/privacy/molcajete.html
