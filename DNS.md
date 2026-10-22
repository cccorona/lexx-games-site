# CNAME lexx.games → GitHub Pages

## Cuándo

Cuando controles el DNS de `lexx.games` y quieras URLs canónicas tipo:

- `https://lexx.games/privacy`
- `https://lexx.games/privacy/molcajete.html`
- `https://lexx.games/support`
- `https://lexx.games/terms`
- `https://lexx.games/credits/molcajete.html`

## Pasos

1. En el repo: crea archivo `CNAME` en la raíz con una sola línea:

   ```
   lexx.games
   ```

   (Si usáis `www.lexx.games`, poned ese host y redirigid apex en el DNS.)

2. En el proveedor DNS:

   - **Apex** `lexx.games`: registros A de GitHub Pages (IPs actuales en [docs de GitHub](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)), **o** ALIAS/ANAME si el DNS lo soporta.
   - **www** (opcional): CNAME → `<user>.github.io`

3. GitHub → Settings → Pages → Custom domain → `lexx.games` → Enforce HTTPS.

4. Actualizad `docs/legal/` en cada juego a la URL `https://lexx.games/...`.

## Mientras tanto

Usad `https://<user>.github.io/lexx-games-site/...` en fichas de tienda y docs.
