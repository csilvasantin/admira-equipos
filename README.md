# Admira Equipos

Inventario de ordenadores de las sedes de Admira, organizado por ubicación.

## Estructura

```
data/
├── sedes.json              # Lista de sedes
└── equipos/
    ├── barcelona.json      # Equipos de Barcelona
    └── sitges.json         # Equipos de Sitges
```

## Uso

Cada archivo en `data/equipos/` contiene un array de equipos con:
- Identificador de máquina
- Nombre, tipo y plataforma
- Usuario asignado y rol
- Especificaciones técnicas (cuando se conozcan)
- Notas operativas

## Relación con otros repos

- **AdmiraNext-Team**: panel de estado en tiempo real. Este repo es el inventario estático de referencia.
- **onboarding**: el welcome pack enlaza aquí para que nuevas IAs conozcan el parque de máquinas.
