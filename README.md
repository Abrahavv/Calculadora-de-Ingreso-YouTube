# Cálculadora de Ingreso YouTube

Estima tus ganancias mensuales de YouTube usando **Vistas** y **RPM** (Revenue Per Mille).

![MIT License](https://img.shields.io/badge/license-MIT-red)
![Version](https://img.shields.io/badge/version-1.0-blue)

## Demo

Abre `index.html` en tu navegador. No requiere instalación.

## Características

- **Cálculo en tiempo real** de ingresos mensuales
- **Gráfico de escenarios** con 5 niveles de vistas (10K a 1M)
- **Tooltips informativos** sobre RPM y vistas
- **Diseño responsive** (móvil, tablet, desktop)
- **Favicon** personalizado

## Fórmula

```
Ingreso = (Vistas ÷ 1,000) × RPM
```

**RPM** (Revenue Per Mille) = Ganancia por cada 1,000 vistas. Varía según nicho ($2–$10 promedio).

## Arquitectura SOLID

El JavaScript está refactorizado siguiendo los principios SOLID:

| Clase | Principio | Responsabilidad |
|---|---|---|
| `Constants` | SRP | Configuración centralizada |
| `IncomeCalculator` | SRP | Fórmula pura de cálculo |
| `InputValidator` | SRP | Validación de entradas |
| `InputParser` | SRP | Sanitización de strings |
| `CurrencyFormatter` | SRP | Formateo de moneda |
| `UIManager` | SRP | Actualización de interfaz |
| `ChartManager` | SRP | Ciclo de vida de Chart.js |
| `App` | DIP/OCP | Orquestador con inyección de dependencias |

## Tecnologías

- **HTML/CSS** — Tailwind-free, diseño custom
- **JavaScript** — ES6+ (clases, privados con `#`)
- **Chart.js 4.4.0** — Gráficos de barras
- **Inter** — Tipografía (Google Fonts)

## Uso

1. Ingresa las **vistas totales al mes**
2. Ingresa tu **RPM** (ingreso por cada 1,000 vistas)
3. El resultado se muestra automáticamente
4. El gráfico muestra comparación con otros escenarios

## Licencia

[MIT](LICENSE) © 2026 USUARIO
