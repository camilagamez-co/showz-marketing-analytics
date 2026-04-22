# Showz — Optimización de Marketing Spend

> USD 329K invertidos en marketing. ROMI global: -7%.  
> Este análisis identifica dónde se pierde el dinero y cómo redistribuirlo sin gastar un dólar más.

---

## 🎯 Problema de negocio

Showz, plataforma de venta de entradas para eventos de entretenimiento, invirtió USD 329,131 en marketing durante 12 meses sin claridad sobre qué canales generaban retorno real. El 42.9% del presupuesto se concentraba en una sola fuente con ROMI de -61%, mientras canales con ratios LTV/CAC superiores a 6.0 recibían menos del 36% combinado.

---

## 🛠️ Herramientas usadas

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Estadística descriptiva e inferencial
- SciPy

---

## 🔍 Metodología

- Limpieza y estandarización de 3 datasets: 359,400 visitas, 50,415 pedidos, 2,542 registros de costos
- Cálculo de métricas de usuario: DAU, WAU, MAU, duración de sesión, sticky factor
- Análisis de cohortes de retención y conversión por fuente de adquisición
- Cálculo de LTV, CAC y ROMI por canal y por dispositivo
- Economía unitaria: comparación LTV/CAC con benchmark ≥ 3.0
- Simulación de escenario de redistribución presupuestal sin incrementar gasto total

---

## 💡 Hallazgo principal

Source 3 absorbe el 42.9% del presupuesto (USD 141,322) con un ROMI de -61%, mientras Source 5 opera con LTV/CAC de 7.23 —el mejor del portafolio— recibiendo apenas el 15.7% de la inversión.

---

## 📊 Impacto o decisión que genera

Redistribuir el presupuesto existente hacia Sources 4, 5 y 1 —sin incrementar el gasto total— proyecta un cambio de ROMI de -7% a +18% en 90 días, convirtiendo una pérdida mensual de USD 1,918 en una ganancia de USD 4,940. La recomendación incluye un plan de acción por semanas con KPIs de monitoreo.

---

## ▶️ Cómo correr el código

```bash
git clone https://github.com/tu-usuario/showz-marketing-analytics
cd showz-marketing-analytics
pip install -r requirements.txt
jupyter notebook Showz_-_Optimización_de_Marketing_Spend.ipynb
```

**Datasets requeridos** (colocar en carpeta `/datasets/`):
- `visits_log_us.csv`
- `orders_log_us.csv`
- `costs_us.csv`
