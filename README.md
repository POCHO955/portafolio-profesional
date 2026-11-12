# Tu Portafolio Profesional en Vercel

Aprende Git en VS Code, conecta GitHub y despliega tu CV o portafolio paso a paso.

Disponible para estudiantes
Noviembre 2026

## ¿Qué vas a lograr con esta guía?

Al terminar esta guía tendrás tu portafolio profesional o CV desplegado en internet, con una URL pública que podrás compartir en tu currículum, LinkedIn o con reclutadores. Aprenderás a usar Git desde Visual Studio Code, a subir tu código a GitHub y a desplegarlo automáticamente en Vercel.

Git en VS Code

Control de versiones visual

GitHub

Repositorio remoto de tu código

Vercel

Despliegue automático en la nube

PASO 1
## Preparar el entorno

Antes de comenzar, asegúrate de tener instalado:

1. Git

Descárgalo de git-scm.com

2. VS Code

code.visualstudio.com

3. Cuenta GitHub

github.com (gratis)

Verificación: Abre VS Code, ve a la barra lateral izquierda y busca el icono de Source Control (parece una bifurcación). Si lo ves, Git está listo.

PASO 2
## Crear la carpeta de tu portafolio

Crea una carpeta en tu escritorio llamada mi-portafolio y dentro crea estos archivos:

```text
mi-portafolio/
├── index.html    ← Tu página principal
├── styles.css    ← Los estilos
└── README.md     ← Descripción del proyecto
```

Crea un index.html básico con tu nombre, foto, habilidades y proyectos. Puedes usar cualquier plantilla o crear la tuya. Lo importante es que tengas algo que mostrar.

Tip: Si no sabes por dónde empezar, busca "portfolio template HTML CSS" en Google o usa generadores como el paquete `@panchito4044/portfolio-template`.

PASO 3
## Inicializar Git en VS Code

Abre VS Code y sigue estos pasos:

1. Abre la carpeta mi-portafolio en VS Code (`Archivo → Abrir carpeta`).
2. Haz clic en el icono de Source Control en la barra lateral izquierda (o presiona `Ctrl + Shift + G`).
3. Haz clic en "Initialize Repository" (Inicializar repositorio).
4. Verás que todos tus archivos aparecen con una letra U (Untracked = no rastreados).

¿Qué acaba de pasar? Se creó una carpeta oculta `.git` dentro de tu proyecto. Git ahora "vigila" los cambios en tus archivos.

PASO 4
## Hacer tu primer commit

Un commit es una "foto" de tu proyecto en un momento dado. Sigue estos pasos:

1. En el panel de Source Control, pasa el mouse sobre la sección Changes y haz clic en el icono + (Stage All Changes). Esto prepara todos los archivos para el commit.
2. Arriba, en el cuadro de texto, escribe un mensaje descriptivo: `Primer commit: estructura inicial del portafolio`.
3. Haz clic en el botón ✓ Commit (o presiona `Ctrl + Enter`).

Resultado: Los archivos desaparecen de "Changes". Tu proyecto está guardado en el historial de Git local.

PASO 5
## Conectar tu proyecto con GitHub

Ahora subiremos tu código a GitHub, que es como un "Google Drive para programadores".

1. En el panel de Source Control, haz clic en los tres puntos (...) junto a "Changes".
2. Selecciona "Publish Branch" (Publicar rama).
3. VS Code te pedirá iniciar sesión con GitHub. Autoriza el acceso.
4. Elige un nombre para tu repositorio: `mi-portafolio`.
5. Selecciona si será público (recomendado para portafolio) o privado.
6. Haz clic en Publish.

Alternativa: Si ya tienes un repositorio en GitHub, usa `Git: Add Remote` desde la paleta de comandos (`Ctrl + Shift + P`) y pega la URL de tu repositorio.

PASO 6
## Crear cuenta en Vercel y conectar GitHub

1. Ve a vercel.com y haz clic en Sign Up.
2. Selecciona "Continue with GitHub" (recomendado). Esto vincula automáticamente tus repositorios.
3. Autoriza a Vercel para acceder a tu cuenta de GitHub.
4. Elige el plan Hobby (gratis).
5. Personaliza tu nombre de usuario (ej: `tu-nombre`). Este será parte de tu URL: `tu-nombre.vercel.app`.

Importante: Usa el mismo nombre de usuario en GitHub, Vercel y LinkedIn para construir tu marca personal.

PASO 7
## Desplegar tu portafolio

Una vez dentro de tu dashboard de Vercel:

1. Haz clic en "Add New... → Project".
2. Verás una lista de tus repositorios de GitHub. Busca mi-portafolio y haz clic en Import.
3. Vercel detectará automáticamente que es un proyecto estático (HTML/CSS).
4. Haz clic en Deploy.
5. Espera unos segundos mientras Vercel construye y publica tu sitio.

¡Listo! Vercel te mostrará una URL como `https://mi-portafolio-tu-nombre.vercel.app`. Esa es tu página en vivo. Haz clic en "Visit" para verla.

PASO 8
## Actualizar tu portafolio (flujo continuo)

Cada vez que quieras actualizar tu portafolio (agregar un proyecto, cambiar tu foto, etc.), el flujo es:

```text
1. Editas tus archivos en VS Code
2. Guardas los cambios (Ctrl + S)
3. En Source Control, escribes un mensaje de commit
4. Haces clic en ✓ Commit
5. Haces clic en "Sync Changes" (o Push)
6. Vercel detecta el cambio y redespliega AUTOMÁTICAMENTE
```

Magia de Vercel: No necesitas hacer nada más. Cada vez que subas cambios a GitHub, Vercel reconstruirá tu sitio en segundos. Tu URL sigue siendo la misma.

PASO 9
## Personalizar tu URL (opcional)

Vercel te da una URL por defecto, pero puedes cambiarla por algo más profesional:

1. En tu proyecto de Vercel, ve a Settings → Domains.
2. Verás tu URL actual. Haz clic en Edit.
3. Puedes cambiar el subdominio (ej: `tu-nombre.vercel.app`).
4. Si tienes un dominio propio (ej: `tunombre.com`), puedes agregarlo aquí. Vercel te guiará para configurar los DNS.

## Resumen del Flujo Completo

```text
TU COMPUTADORA                    GITHUB                    VERCEL

VS Code                              Repositorio              Plataforma
   │                                    │                        │
   │ 1. Creas archivos                  │                        │
   │ 2. Inicializas Git                 │                        │
   │ 3. Haces Commit                    │                        │
   │ 4. Publish Branch ───────────────► │                        │
   │                                    │ 5. Conectas cuenta ──► │
   │                                    │                        │ 6. Importas proyecto
   │                                    │                        │ 7. Deploy automático
   │                                    │                        │
   │ 8. Editas archivos                 │                        │
   │ 9. Commit + Sync ────────────────► │                        │
   │                                    │ 10. Detecta cambio ──► │
   │                                    │                        │ 11. Redespliega
   │                                    │                        │
   ▼                                    ▼                        ▼
                                                                  🌐 URL PÚBLICA
```

Local

Editas y commiteas

GitHub

Almacena tu código

Vercel

Publica en internet

## Consejos para que tu portafolio destaque

Sí hacer

- Incluye una foto profesional.
- Muestra 3-4 proyectos con capturas y enlaces.
- Explica qué tecnologías usaste en cada proyecto.
- Agrega tu email y LinkedIn de contacto.
- Mantén el diseño limpio y responsive.

Evitar

- Dejar texto de ejemplo ("Lorem ipsum").
- Poner proyectos que no puedes explicar.
- Usar imágenes de baja calidad.
- Olvidar el enlace a tu GitHub.
- Hacerlo solo para escritorio (debe verse en móvil).

---

## Proyecto actual

Este repositorio incluye una landing page de portafolio profesional lista para publicar en Vercel. Personaliza los textos, nombre, contacto y proyectos en `index.html` y luego súbelo a GitHub para desplegarlo con Vercel.
