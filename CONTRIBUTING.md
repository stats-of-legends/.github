# Contribuer à Stats Of Legends

## Flux de travail
- **Trunk-based** : `main` est toujours déployable. Branches courtes (< 3 jours) : `feat/<contexte>-<sujet>`, `fix/…`, `chore/…`, `docs/…`.
- Fonctionnalité incomplète → derrière un feature flag.
- Fusion par **squash** ; le titre de la PR devient le message du commit.

## Commits et titres de PR
[Conventional Commits](https://www.conventionalcommits.org/fr/) : `type(portée): description` — types `feat`, `fix`, `chore`, `docs`, `refactor`, `test`, `perf`, `ci`. La portée est le bounded context (`stats-lol`, `riot-client`, `ui`…).

## Definition of Done
- Code + tests (seuils de couverture respectés).
- Contrats (`packages/contracts`) à jour si l'API change.
- Documentation / ADR à jour si une décision structurante change.
- Accessibilité vérifiée (axe) pour toute UI.
- Logs et métriques ajoutés si nouveau flux.
- Migration compatible N-1 si le schéma change.
- Registre RGPD à jour si une donnée personnelle est ajoutée.

## Architecture
Le dossier d'architecture (`docs/architecture/` dans `sol-platform`) et les ADR (`docs/adr/`) font référence. Les frontières entre modules sont vérifiées en CI.

## Code généré par IA
Même exigence de revue que le reste. Aucune donnée de production ni secret dans les prompts. Suivre `AGENTS.md` de chaque dépôt.
