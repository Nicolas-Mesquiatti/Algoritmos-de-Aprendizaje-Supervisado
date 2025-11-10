# 📊 Árbol de Decisión – Predicción de aceptación de oferta

Este proyecto aplica técnicas de aprendizaje automático para construir un árbol de decisión que predice si un cliente aceptará una oferta de plan de datos móviles, usando un conjunto de datos de una empresa de telecomunicaciones.

---

## 🧠 Objetivo

Determinar qué atributo permite clasificar con mayor precisión la decisión del cliente respecto a la oferta, y construir un árbol de decisión paso a paso.

---

## 📁 Datos utilizados

El conjunto incluye 10 clientes con los siguientes atributos:

- Edad (agrupada: Joven ≤30, Adulto 31–50, Mayor >50)
- Uso mensual de datos (agrupado: Bajo ≤3GB, Medio 3.1–6GB, Alto >6GB)
- Tiene línea fija (Sí / No)
- Aceptó la oferta (Sí / No)

---

## 📈 Resultados del análisis

### 🔹 Entropía del conjunto original

- Entropía total: **1.000** (máxima incertidumbre)

### 🔹 Ganancia de información por atributo

| Atributo           | Agrupación usada                          | Ganancia de información |
|--------------------|-------------------------------------------|--------------------------|
| Tiene línea fija   | Sí / No                                   | **1.000** ✅  
| Uso de datos       | Bajo / Medio / Alto                       | 0.600  
| Edad               | Joven / Adulto / Mayor                    | 0.449  

---

## 🌳 Árbol de decisión construido

```text
¿Tiene línea fija?
├── No → Rechaza la oferta
└── Sí → Acepta la oferta
