# challege-telecomX1
# 📊 Análisis de Churn en TelecomX

Este proyecto tiene como objetivo analizar los datos de clientes de **TelecomX** con el fin de identificar patrones que expliquen la pérdida de clientes (Churn) y proponer **estrategias de mejora del servicio** orientadas a la retención y fidelización.

---

## 📂 Contenido del Proyecto

- `Challenge_telecomX.ipynb`: Notebook original del reto de análisis.
- `TelecomX_Alternativo.ipynb`: Versión alternativa del análisis (misma lógica, diferente camino).
- `README.md`: Documento de referencia del proyecto.
- `data/`: Carpeta con la fuente de datos utilizada (JSON desde repositorio externo).

---

## 📌 Contexto

En la industria de las telecomunicaciones, **la deserción de clientes (Churn)** representa uno de los principales desafíos estratégicos.  
Conocer **qué factores influyen en la decisión de cancelar un servicio** permite a la empresa **optimizar su oferta, mejorar la experiencia del cliente y aumentar los ingresos recurrentes**.

---

## 🎯 Objetivos

1. **Analizar los datos de clientes de TelecomX** para identificar patrones de cancelación.  
2. **Detectar variables críticas** que influyen en la permanencia (contratos, métodos de pago, soporte técnico, etc.).  
3. **Proponer estrategias de mejora del servicio** enfocadas en retención y satisfacción del cliente.  

---

## 📊 Dataset

- **Fuente:** [TelecomX Data JSON](https://raw.githubusercontent.com/ingridcristh/challenge2-data-science-LATAM/refs/heads/main/TelecomX_Data.json)  
- **Formato:** JSON, normalizado a DataFrame en Python.  
- **Variables principales:**
  - `Churn`: Variable objetivo (cliente se da de baja: sí/no).  
  - `account.Charges.Total`: Cargos totales acumulados.  
  - `account.Contract`: Tipo de contrato (mensual, anual, bianual).  
  - `account.PaymentMethod`: Método de pago utilizado.  
  - `internet.*`: Servicios asociados al internet (backup, soporte, streaming, etc.).  
  - `customer.*`: Información demográfica básica.  

---

## 🛠️ Metodología

1. **Carga y normalización de datos** desde JSON.  
2. **Limpieza de datos:**
   - Conversión de variables numéricas.  
   - Manejo de valores nulos.  
   - Normalización de strings.  
3. **Análisis exploratorio (EDA):**
   - Distribución de clientes por churn.  
   - Relación entre cargos, contratos y métodos de pago.  
   - Impacto de servicios adicionales en la retención.  
4. **Visualización:**
   - Histogramas y gráficos de barras con `matplotlib` y `seaborn`.  
   - Visualización interactiva con `plotly`.  
5. **Interpretación estratégica:**
   - Identificación de factores clave.  
   - Propuestas de acción empresarial.  

---

## 🔎 Hallazgos Clave

- La variable **contrato** es determinante: los clientes con contratos flexibles (mensuales) tienden a cancelar más que los contratos a largo plazo.  
- Los clientes que cuentan con **servicios adicionales** (ej. streaming, respaldo en línea, soporte técnico) presentan **menor tasa de churn**.  
- Los problemas relacionados con **métodos de pago y facturación** impactan de manera significativa en la deserción.  
- El costo total **no es el principal motivo de cancelación**: la **calidad de servicio y sopor**
