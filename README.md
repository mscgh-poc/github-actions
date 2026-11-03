# github-actions

Acciones compuestas reutilizables para la organización **mscgh-poc**.

## Acciones disponibles

| Acción | Descripción |
|---|---|
| `actions/setup-node-project` | Configura Node.js y restaura dependencias con caché |
| `actions/deploy-summary` | Genera un Job Summary con datos del despliegue |

## Uso

```yaml
- uses: mscgh-poc/github-actions/actions/setup-node-project@main
  with:
    node-version: '22'
```

## Convenciones

- Cada acción vive en `actions/<nombre>/action.yml`
- Usar acciones oficiales directamente cuando no hay política propia que encapsular
- Fijar dependencias a SHA inmutables en las acciones oficiales
