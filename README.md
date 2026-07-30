# Am'Arte Vital Flow

Sitio web estático para Am'Arte Vital Flow — acompañamiento integrativo en naturopatía, movimiento consciente y talleres de bienestar.

## Desarrollo

```bash
npm install
npm run dev
```

Abre [http://localhost:4321](http://localhost:4321).

## Build

```bash
npm run build
npm run preview
```

## Deployment

This repo deploys automatically to Gandi hosting via **SFTP** using a GitHub Action workflow: `.github/workflows/deploy-gandi-sftp.yml`.

- **When it runs**: on every push to the `main` branch
- **What it does**: installs dependencies, runs `npm run build`, then uploads the contents of `dist/`

Required GitHub repository secrets:

| Secret | Description |
| --- | --- |
| `SFTP_SERVER` | Gandi SFTP host |
| `SFTP_USERNAME` | SFTP username |
| `SFTP_PASSWORD` | SFTP password |
| `SFTP_REMOTE_PATH` | Remote directory for this site |

## Estructura

- `src/data/site.ts` — todo el contenido editable (textos, contacto, servicios)
- `src/pages/` — páginas del sitio
- `src/components/` — componentes reutilizables
- `public/logo.png` — logo de marca

## Pendiente

- Fotos reales (Alizé, espacio, talleres)
- Datos de contacto definitivos
- Textos legales completos
- Conexión del formulario de contacto
- Tienda (página provisional)
- Testimonios reales
