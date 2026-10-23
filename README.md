# Retail Intelligence

Proyecto de análisis de datos — UCAB, Tópicos Especiales.

## Objetivo

Analizar los datos de una empresa de retail (clientes, transacciones, productos, devoluciones, interacciones de CRM y campañas de marketing) para generar hallazgos accionables respaldados por análisis estadístico y presentarlos en un tablero de Power BI.

## Estructura

```
retail-intelligence/
├── data/
│   ├── raw/        # CSV originales (NUNCA se editan)
│   └── clean/      # Datos limpios generados por los notebooks
├── notebooks/      # Análisis en Jupyter (un dueño por notebook)
├── powerbi/        # Archivo .pbix del tablero
├── docs/
│   ├── bitacora_ia.md   # Registro del uso de IA
│   └── decisiones.md    # Registro de decisiones
├── requirements.txt
└── README.md
```

### Datos de origen (`data/raw/`)

| Archivo | Contenido |
|---|---|
| `clientes.csv` | Clientes |
| `transacciones.csv` | Transacciones de venta |
| `productos.csv` | Catálogo de productos |
| `devoluciones.csv` | Devoluciones |
| `interacciones_crm.csv` | Interacciones de CRM |
| `campanas_marketing.csv` | Campañas de marketing |

## Equipo

| Integrante | Rol |
|---|---|
| HannerDev | Datos y análisis |
| Ana | Historia, defensa y dashboard de Power BI (D11) |
| Adrián | Documentación de calidad |
| JH | Validador |
| Andrés | Presentación |

## Instalación

```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS / Linux
source .venv/bin/activate

pip install -r requirements.txt
```

## Reglas

1. **Un dueño por notebook.** Solo su dueño lo edita; los demás comentan o proponen cambios.
2. **`data/raw/` nunca se edita.** Toda limpieza se hace en notebooks y se guarda en `data/clean/`.
3. **El `.pbix` solo lo toca Ana (D11).**
4. Todo uso de IA se registra en `docs/bitacora_ia.md`.
5. Toda decisión relevante se registra en `docs/decisiones.md`.
