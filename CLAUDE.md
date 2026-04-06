# Proyecto 07 — Admira Equipos

> Inventario de ordenadores de las sedes de Admira, organizado por ubicación.

## Contexto

Base de datos estática (JSON) de todas las máquinas en las sedes Admira:
- **Barcelona**: AdmiraNext, AdmiraXtore, AdmiraXperience, AdmiraXpace, Admira University
- **Sitges**: Admira Sitges

Cada máquina registra identificador, nombre, tipo, plataforma, usuario asignado, rol, especificaciones y notas operativas.

## Arquitectura

```
admira-equipos/
├── data/
│   ├── sedes.json                    # Registro maestro de todas sedes
│   └── equipos/
│       ├── admira-next.json          # Barcelona
│       ├── admira-xtore.json         # Barcelona
│       ├── admira-xperience.json     # Barcelona
│       ├── admira-xpace.json         # Barcelona
│       ├── admira-university.json    # Barcelona
│       └── sitges.json               # Sitges
└── README.md
```

Cada equipo incluye:
- Identificador de máquina
- Nombre, tipo, plataforma
- Usuario asignado y rol
- Especificaciones técnicas
- Notas operativas

## Notas para IAs

1. **Propósito**: Inventario estático de referencia. No es panel en tiempo real (ese es AdmiraNext-Team).

2. **Relación con otros proyectos**:
   - **AdmiraNext-Team** (Proyecto 03): Panel dinámico de estado. Usa este inventario como fuente de máquinas conocidas.
   - **Onboarding** (Proyecto 06): Nuevas IAs consultan aquí para conocer el parque disponible.

3. **Mantenimiento**: Actualizar cuando se añaden/retiran máquinas o se cambian asignaciones de usuario/rol.

4. **Próximos pasos**: Sincronización automática con AdmiraNext-Team, API de consulta por sede/tipo/usuario, histórico de cambios.
