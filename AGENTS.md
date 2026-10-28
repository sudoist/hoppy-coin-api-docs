# Hoppy Coin API Docs — Agent Guidance

Maintain an accurate, minimal API reference for the experimental Hoppy Coin game.

- Use `master` as the PR target. Do not push to `master` or merge without owner approval.
- Keep `swagger.yaml` aligned with the actual Laravel routes, validation, and responses; never invent endpoints or claim runtime verification without tests.
- Do not publish actual API keys. Explain that browser-delivered keys are public.
- Preserve Swagger UI third-party notices and avoid automatic dependency upgrades without a reason.
- No staging infrastructure or permanent `develop` branch. Keep changes small.
