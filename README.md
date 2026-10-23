# Panel de aplicaciones (juancandanedo.org)

Para agregar una app: edita `apps.js` (copia un bloque, cambia nombre, descripción, `url`, `estado: 'activa'`) y vuelve a arrastrar la carpeta a Netlify (Deploys).

## Poner el dominio (comprado en Netlify, el DNS ya lo maneja Netlify)
Orden recomendado para no tumbar el examen:
1. **Examen:** abre el sitio actual del examen → Domain management. Agrega `examen.juancandanedo.org` como dominio y, cuando quede activo, quita `juancandanedo.org` de ese sitio (o márcalo como no principal).
2. **Presupuestos:** sitio de presupuestos → Domain management → Add domain → `presupuestos.juancandanedo.org`.
3. **Panel:** en https://app.netlify.com/drop arrastra esta carpeta → nuevo sitio → Domain management → Add domain → `juancandanedo.org` (principal). Opcional: también `www.juancandanedo.org`.
4. Netlify crea los registros DNS de cada subdominio y el certificado HTTPS solo (puede tardar unos minutos).
5. Si activas el inicio de sesión con Google en Presupuestos, agrega `https://presupuestos.juancandanedo.org` a los «Orígenes de JavaScript autorizados» del ID de cliente.
