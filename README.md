# Hoppy Coin API documentation

Swagger UI documentation for the [Hoppy Coin Laravel API](https://github.com/sudoist/hoppy-coin-api), used by the [Phaser game](https://github.com/sudoist/hoppy-coin).

The previous specification was an unmodified Petstore example. The current `swagger.yaml` describes the known v1 score endpoints; it should be updated alongside API behavior changes.

## API endpoints

- `GET /api/v1/scores?level=Ranked1` — retrieve scores for a level.
- `POST /api/v1/scores` — submit `name`, `score`, and `level` as JSON.
- Both require the `x-api-key` header. Keys distributed with the browser game are public and do not provide anti-cheat protection.

The actual response structure and status codes should be checked against the running Laravel API before treating this as a production-verified contract.

## Maintenance

The Swagger UI assets are stored in this repository. A GitHub Actions workflow may propose UI dependency updates; review rather than automatically merge them. Keep docs changes small, open PRs against `master`, and avoid unnecessary dependency churn. See [AGENTS.md](AGENTS.md).

## Licensing

Swagger UI assets retain their upstream licenses. Licensing for original Hoppy Coin code and documentation requires separate owner confirmation.
