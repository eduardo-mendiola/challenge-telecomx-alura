# Challenge Alura Latam - G8 ONE
## Telecom X - Análisis de Evasión de Clientes

## Propósito del Proyecto

Este proyecto analiza la **evasión de clientes (churn)** en una empresa de telecomunicaciones con el objetivo de identificar patrones y factores que influyen en la pérdida de clientes. El análisis busca generar insights para diseñar estrategias que reduzcan el churn y mejoren la fidelización.

## Estructura del Proyecto

- `TelecomX_LATAM.ipynb` : Notebook principal con el análisis completo, incluyendo limpieza de datos, análisis exploratorio y visualizaciones.
- `data/` : Carpeta que contiene los archivos de datos originales y procesados.
- `README.md` : Este archivo, que describe el proyecto y cómo usarlo.


## Instrucciones para Ejecutar el Notebook

1. Clona este repositorio:
   ```bash
   git clone https://github.com/https://github.com/eduardo-mendiola/challenge-telecomx-alura
   cd telecom-x

# Informe Final – Análisis de Evasión de Clientes (Churn)

## Introducción

Este análisis aborda el problema de la **evasión de clientes (churn)** en una empresa de telecomunicaciones. El objetivo principal es identificar patrones y características comunes entre los clientes que abandonan el servicio, para desarrollar estrategias efectivas que reduzcan la pérdida de clientes y fortalezcan su fidelización.

---

## Limpieza y Tratamiento de Datos

Se aplicaron los siguientes pasos para preparar los datos:

- **Importación y exploración** inicial de los datos.
- **Renombrado de columnas** para eliminar símbolos innecesarios y estandarizar nombres.
- Conversión de variables categóricas binarias (`Yes` / `No`) a valores numéricos (`1` / `0`).
- Conversión de columnas numéricas con tipo incorrecto (como `charges_total`) a `float`.
- Creación de la nueva columna **`cuentas_diarias`**, a partir de la facturación mensual dividida por 30, para obtener una visión del gasto diario promedio del cliente.

---

## Análisis Exploratorio de Datos

### Distribución General del Churn

El análisis muestra que aproximadamente **el 27% de los clientes se dieron de baja**, mientras que el **73% permanecieron activos**.

### Evasión por Variables Categóricas

Se exploraron variables como:

- **Género**
- **Tipo de contrato**
- **Método de pago**
- **Servicios digitales adicionales**

**Hallazgos**:
- Mayor evasión entre quienes tienen contratos **mes a mes**.
- **Pagos mediante cheque electrónico** se asocian con más evasión.
- Clientes **sin servicios complementarios** tienen mayor propensión a cancelar.

### Evasión por Variables Numéricas

Se analizaron principalmente las siguientes columnas numéricas:

- **`tenure`** (antigüedad en meses): los clientes que se van tienden a tener menor antigüedad.
- **`charges_total`** (gasto total): clientes con menor gasto total tienen una mayor tasa de churn.
- **`cuentas_diarias`**: clientes con menor gasto diario presentan una leve tendencia a abandonar.

---

## Conclusiones e Insights

- **Contratos cortos y clientes nuevos** tienen mayor riesgo de churn.
- La ausencia de **servicios adicionales** puede ser un factor que disminuye el compromiso del cliente.
- Los **métodos de pago automatizados** podrían ayudar a reducir la evasión.
- Las variables numéricas refuerzan la idea de que los clientes menos comprometidos (por tiempo o inversión) abandonan con más frecuencia.

---

## Recomendaciones Estratégicas

1. **Incentivar contratos a largo plazo** mediante beneficios o descuentos exclusivos.
2. **Implementar campañas de retención temprana**, enfocadas en clientes nuevos.
3. **Promover servicios adicionales** (ej: soporte técnico, protección de dispositivos).
4. **Fomentar el uso de pagos automáticos** mediante incentivos económicos.
5. **Desarrollar modelos predictivos de churn** para actuar preventivamente frente a clientes en riesgo.

---

