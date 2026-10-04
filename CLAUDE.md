# CLAUDE.md — awesome-comunitat-valenciana

## Propósito

Selección de software open source que da **soporte específico a la Comunitat Valenciana** — su gobierno autonómico (GVA), ayuntamientos, universidades, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco es la Comunitat Valenciana: el software debe dirigirse específicamente a esta comunidad autónoma o a sus municipios.

## Ámbito

- **3 provincias**: Alacant/Alicante, Castelló/Castellón, València/Valencia.
- Principales ciudades: València (capital), Alacant, Castelló de la Plana, Elx, Benidorm, Torrevieja, Gandia, Alcoi, Sagunt, Dénia, Xàtiva, Orihuela, Vila-real, Elda, Ontinyent, Alzira, Novelda, Villena, Sueca, Oliva.
- **Universidades**: UV (Universitat de València), UPV (Universitat Politècnica de València), UA (Universitat d'Alacant), UJI (Universitat Jaume I de Castelló), UMH (Universitat Miguel Hernández d'Elx).
- **Instituciones**: GVA (Generalitat Valenciana), IVACE (Institut Valencià de Competitivitat Empresarial), IVE (Institut Valencià d'Estadística), CEICE (Conselleria d'Educació, Universitats i Ocupació), LliureX (distribución GNU/Linux educativa de la GVA), FGV (Ferrocarrils de la Generalitat Valenciana).

## Criterios de inclusión

### Incluir

- Software que interactúa con la **GVA** o sus organismos (Sede Electrónica, Portal de Transparencia, datos abiertos, Aules, LliureX).
- Herramientas para **ayuntamientos** de la Comunitat Valenciana.
- Software de **universidades valencianas** (UV, UPV, UA, UJI, UMH) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** de la Comunitat Valenciana (dadesobertes.gva.es, IVE).
- Software relacionado con **LliureX**, la distribución educativa de la GVA.
- Herramientas de **transporte** valenciano (MetroValencia, EMT Valencia, TRAM Alacant, FGV, ValenBisi).
- Software sobre **fiestas y patrimonio** de la región (Fallas, Fogueres, Magdalena).
- Herramientas de **turismo y costa** de la Comunitat Valenciana.
- Software de **agricultura e innovación** regional (IVACE, IVIA).
- Herramientas de **cartografía y SIG** específicas de la Comunitat Valenciana.
- Proyectos del **sistema sanitario valenciano**.
- Software **educativo** específico de la región (Aules, centros educativos).
- Herramientas de **medio ambiente** regional (l'Albufera, parques naturales).
- Proyectos de **smart cities** para ciudades valencianas.
- Herramientas de **participación ciudadana** de la GVA o ayuntamientos valencianos.

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de la Comunitat Valenciana — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por valencianos que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de universidades valencianas que podrían ser genéricos — incluir si tienen datos o configuración específica de la Comunitat Valenciana.
- Software que cubre la Comunitat Valenciana junto con otras regiones — incluir si la Comunitat Valenciana es un foco principal.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución valenciana** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-comunitat-valenciana» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades valencianas (Reddit, foros de la UV/UPV/UA, Telegram de devs valencianos, VLCTechHub) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- **LliureX** es la distribución GNU/Linux educativa de la GVA con una organización GitHub `lliurex` muy activa (80+ repos). `lliurex-store` (8 estrellas) es el repo principal. Muchos repos son componentes internos sin README ni estrellas.
- **VLCTechHub** es la comunidad tecnológica de Valencia con repos activos: `VLCTechHub-site` (26 estrellas), `VLCTechHub-api` (5 estrellas).
- **EMT Valencia**: `ElEd0/EMTValencia-API` (14 estrellas) es el módulo Python más popular para consultar horarios de bus.
- **MetroValencia**: `luisnomad/metrovalencia` (5 estrellas) y `legomolina/MetroVlcSchedule` (11 estrellas, archivado) son los repos más relevantes.
- **ValenBisi**: `systemallica/ValenBisi` (7 estrellas) es una app Android funcional.
- La GVA no tiene organización GitHub oficial. Los repos son de desarrolladores independientes.
- `Usabi/consul_gva` es un fork de Consul para participación ciudadana de la GVA.
- El API de búsqueda de GitHub tiene rate limit de 30 req/min — usar `gh api repos/...` (core API, 5000/h) para verificaciones.

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*

<!-- BEGIN BEADS INTEGRATION v:1 profile:minimal hash:6cd5cc61 -->
## Beads Issue Tracker

This project uses **bd (beads)** for issue tracking. Run `bd prime` to see full workflow context and commands.

### Quick Reference

```bash
bd ready              # Find available work
bd show <id>          # View issue details
bd update <id> --claim  # Claim work
bd close <id>         # Complete work
```

### Rules

- Use `bd` for ALL task tracking — do NOT use TodoWrite, TaskCreate, or markdown TODO lists
- Run `bd prime` for detailed command reference and session close protocol
- Use `bd remember` for persistent knowledge — do NOT use MEMORY.md files

**Architecture in one line:** issues live in a local Dolt DB; sync uses `refs/dolt/data` on your git remote; `.beads/issues.jsonl` is a passive export. See https://github.com/gastownhall/beads/blob/main/docs/SYNC_CONCEPTS.md for details and anti-patterns.

## Agent Context Profiles

The managed Beads block is task-tracking guidance, not permission to override repository, user, or orchestrator instructions.

- **Conservative (default)**: Use `bd` for task tracking. Do not run git commits, git pushes, or Dolt remote sync unless explicitly asked. At handoff, report changed files, validation, and suggested next commands.
- **Minimal**: Keep tool instruction files as pointers to `bd prime`; use the same conservative git policy unless active instructions say otherwise.
- **Team-maintainer**: Only when the repository explicitly opts in, agents may close beads, run quality gates, commit, and push as part of session close. A current "do not commit" or "do not push" instruction still wins.

## Session Completion

This protocol applies when ending a Beads implementation workflow. It is subordinate to explicit user, repository, and orchestrator instructions.

1. **File issues for remaining work** - Create beads for anything that needs follow-up
2. **Run quality gates** (if code changed) - Tests, linters, builds
3. **Update issue status** - Close finished work, update in-progress items
4. **Handle git/sync by active profile**:
   ```bash
   # Conservative/minimal/default: report status and proposed commands; wait for approval.
   git status

   # Team-maintainer opt-in only, unless current instructions forbid it:
   git pull --rebase
   git push
   git status
   ```
5. **Hand off** - Summarize changes, validation, issue status, and any blocked sync/commit/push step

**Critical rules:**
- Explicit user or orchestrator instructions override this Beads block.
- Do not commit or push without clear authority from the active profile or the current user request.
- If a required sync or push is blocked, stop and report the exact command and error.
<!-- END BEADS INTEGRATION -->

## Where the tracker syncs

This repo is public, so its tracker syncs only to the private remote named by `sync.remote` in `.beads/config.yaml`. The block above says sync uses "your git remote". Here that never means this GitHub repo. Don't add it as a Dolt remote and don't push `refs/dolt/*` to it.
