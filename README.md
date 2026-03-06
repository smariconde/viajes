# 🌍 Viajes - Información por Destino

Repositorio con información curada de viajes organizada por destino.

## 📁 Estructura

```
viajes/
├── japon-2027/          ← Viaje a Japón (Feb/Mar 2027)
│   ├── itinerario.md    ← Día por día + TOP 10
│   ├── logistica.md     ← Transporte, alojamiento, checklist
│   ├── experiencias.md  ← TOP 20, compras, souvenirs
│   ├── gastronomia.md   ← Restaurantes auténticos
│   ├── presupuesto.md   ← Costos detallados
│   ├── destinos.md      ← Ciudades confirmadas
│   └── notas.md         ← Seguimiento
├── tailandia/           ← Próximo destino
└── europa/              ← Próximo destino
```

## 📄 Archivos por Destino

Cada carpeta de destino contiene:

| Archivo | Contenido |
|---------|-----------|
| `itinerario.md` | Día por día detallado + actividades TOP |
| `logistica.md` | Transporte, alojamiento, visa, apps, checklist |
| `experiencias.md` | TOP 20 atracciones, compras, souvenirs |
| `gastronomia.md` | Restaurantes auténticos + precios |
| `presupuesto.md` | Costos detallados + tips de ahorro |
| `destinos.md` | Ciudades confirmadas + imperdibles |
| `notas.md` | Seguimiento del proyecto |

## 🗾 Destinos Disponibles

### Japón 2027 (`japon-2027/`)
- **Fechas:** Febrero/Marzo 2027
- **Duración:** 14 días
- **Ciudades:** Tokio (6) → Kioto (4) → Osaka (3) → Tokio (1)
- **Presupuesto:** ~$2,400-3,000 USD por persona (todo incluido)
- **Estado:** ✅ Planificación completa

## 🔄 Sincronización

Los archivos se generan automáticamente con el **Skill Viajes** de OpenClaw y se sincronizan con este repo.

### Sincronizar desde workspace:
```bash
# Archivo específico
python3 scripts/github_sync.py japon-2027 itinerario.md

# O todos los archivos de un destino
bash scripts/sync_all.sh japon-2027
```

## 🛠️ Scripts

- `scripts/github_sync.py` — Sincroniza archivos individuales
- `scripts/sync_all.sh` — Sincroniza todos los archivos de un destino

## 📝 Agregar Nuevo Destino

1. Crear carpeta: `mkdir -p /data/workspace/viajes/<destino>/`
2. Generar archivos con el skill de OpenClaw
3. Sincronizar: `bash scripts/sync_all.sh <destino>`

## 🔗 Links

- **GitHub:** https://github.com/smariconde/viajes
- **Skill:** `/data/workspace/skills/viajes/`

---

**Última actualización:** 2026-03-06  
**Mantenido por:** @smariconde
