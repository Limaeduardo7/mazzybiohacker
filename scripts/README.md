# Scripts

Automations and integration helpers live here.

Planned uses:
- weekly content validation/rendering
- Buffer publishing
- asset rendering with Playwright
- document normalization
- safe exports from private operational systems

## Security

Never hardcode tokens. Read secrets from environment variables.

Because this repository is public, any script must be safe to inspect publicly.

## Activation order

1. Configure brand assets.
2. Validate local rendering.
3. Connect Buffer / publishing account.
4. Add idempotent scheduling.
5. Add archive / audit ledger.
