# Landing · José Daniel Cruz Cuba

Sitio estático (HTML + CSS, sin build) con dos demos:

- `/` — landing
- `/demo-ordenes/` — órdenes de trabajo para talleres
- `/demo-reservas/` — reservas con recordatorios por WhatsApp

Las demos guardan los datos solo en el navegador (`localStorage`).

## Ver en local

```bash
python3 -m http.server 8080
```

## Publicar en Cloudflare

Opción A, desde el panel: Workers & Pages → Create → Import a repository → `landing-pymes`.
Build command vacío, deploy command `npx wrangler deploy`. Cada push a `main` se publica solo.

Opción B, desde la terminal:

```bash
npx wrangler deploy
```

Queda en `https://landing-pymes.<tu-subdominio>.workers.dev`.
