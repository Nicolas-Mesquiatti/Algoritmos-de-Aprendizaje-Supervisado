# Regla Inducida y FOIL Gain en Python

Este proyecto implementa en **Python** la generación de reglas inducidas y el cálculo del **FOIL Gain**, con el objetivo de identificar patrones en un conjunto de datos de personas en formación.

---

## 🚀 Contenido del trabajo

1. **Regla inducida para identificar a personas en formación**
   - Identificación de valores únicos en atributos como:
     - **Departamento**
     - **Nivel educativo**
     - **Edad**
   - Respuestas a preguntas guía:
     - No hay departamentos exclusivos en positivos.
     - El nivel educativo **terciario** es común en positivos y no aparece en negativos.
     - Edades exclusivas en positivos: **21, 22, 23 y 24**.

2. **Cálculo del FOIL Gain**
   - Implementación en Python para evaluar condiciones de reglas.
   - Ejemplo:  
     Condición: `nivel_educativo == 'terciario'`
     - FOIL Gain calculado: **3.000**
   - Verificación manual paso a paso.
   - Otra condición evaluada: `edad <= 23`, con mismo resultado de **3.000**.

---

## 📂 Archivos principales

- `FOIL.py` → Programa en Python que calcula el FOIL Gain para diferentes condiciones.
- `README.md` → Descripción del proyecto.

---

## 📊 Interpretación de resultados

- Una regla con **3 positivos y 0 negativos** es muy precisa.
- La ganancia de información (FOIL Gain = 3.000) muestra que la condición es altamente significativa para discriminar positivos.

---

## 🛠️ Requisitos

- Python 3.8+
- No requiere librerías externas (usa operaciones básicas y `math` para logaritmos).

---

python regla_inducida.py
python foil_gain.py
