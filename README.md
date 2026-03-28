# Proto Definitions

Shared protocol buffer definitions for microservices.

## Structure

```
proto-definitions/
├── common/v1/      # Shared types
├── user/        # User service definitions
├── property/    # Property service definitions
└── payment/    # Payment service definitions
```

## Versioning

We use semantic versioning for proto definitions:

- Major: Breaking changes
- Minor: New fields/methods (backward compatible)
- Patch: Documentation updates

## Using in Your Service

### As Git Submodule

```bash
git submodule add https://github.com/fredrickray/propspacex-proto-definitions proto
```

### Updating to Latest

```bash
git submodule update --remote proto
```

## Making Changes

1. Create a feature branch
2. Make your changes
3. Ensure backward compatibility
4. Create PR with clear description
5. After merge, tag the version: `git tag v1.2.0`
