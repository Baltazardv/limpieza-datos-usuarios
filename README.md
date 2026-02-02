# 🧹 Limpieza y Validación de Datos de Usuarios

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

## 🎯 Problema de Negocio

Proporcionar una herramienta sistemática para que Store 1 garantice la coherencia en la recopilación de datos de usuarios. El objetivo es identificar y corregir inconsistencias en formato de nombres, tipos de datos incorrectos y espacios innecesarios que dificultan el análisis de comportamiento de compra y segmentación de clientes.

## 📊 Dataset

- **Registros**: 10 usuarios
- **Variables principales**: user_id, user_name, user_age, fav_categories, total_spendings
- **Fuente**: Datos internos de Store 1
- **Período**: Dataset estático para validación de proceso

**Problemas identificados**:
- ❌ Espacios en blanco al inicio/final de nombres
- ❌ Guiones bajos como separadores en nombres de usuario
- ❌ Edades almacenadas como float en lugar de int
- ❌ Nombres sin separación entre nombre y apellido

## 🛠️ Stack Tecnológico

- **Python 3.9+**: Lenguaje de programación
- **Manipulación de strings**: `strip()`, `replace()`, `split()`
- **Conversión de tipos**: `int()`, `type()`
- **Jupyter Notebook**: Documentación interactiva y análisis

## 📈 Pasos Clave del Proyecto

1. **Análisis de Calidad de Datos**: Evaluación de estructura y tipos de datos
2. **Limpieza de Nombres**: Eliminación de espacios y normalización de separadores
3. **Conversión de Tipos**: Transformación de edades float → int
4. **División de Nombres**: Separación de nombres completos en componentes
5. **Validación**: Verificación de integridad de datos transformados

## ✅ Características y Funcionalidades

✅ **Normalización de Texto**: Limpieza de espacios y estandarización de formatos en nombres  
✅ **Validación de Tipos**: Conversión y verificación de datos numéricos (edades)  
✅ **Estructuración de Datos**: Organización de listas y preparación para análisis  
✅ **Proceso Replicable**: Código documentado para aplicar a futuros lotes de datos  
✅ **Documentación Completa**: Jupyter Notebook con explicaciones paso a paso

## 📊 KPIs y Resultados

### 📈 Resumen General
- **Total de Usuarios Procesados**: 10
- **Edad Promedio**: 30.70 años
- **Rango de Edad**: 22 a 41 años
- **Ingresos Totales**: $9,189.00
- **Gasto Promedio por Usuario**: $918.90

### 🏆 Top Categorías (Por Ingresos)
1. **ELECTRONICS**: $3,160.00
2. **CLOTHES**: $1,865.00
3. **HOME**: $1,546.00
4. **BOOKS**: $986.00
5. **SPORT**: $715.00

### 👥 Perfil Demográfico
- El usuario más joven tiene **22 años** (Jose Martinez)
- El usuario mayor tiene **41 años** (David White)
- La distribución de edad se concentra principalmente en el rango de **20-30 años**

### 💰 Patrones de Gasto
- **Categoría con mayor inversión promedio**: ELECTRONICS ($632.00 por usuario)
- Usuarios que compraron en ELECTRONICS: **5**
- Usuarios que compraron en BOOKS: **4**
- Usuario con mayor gasto total: **Mike Reed** con $1,280.00

### 📌 Estadísticas Adicionales
- **Número promedio de categorías favoritas**: 2.90 por usuario
- **Categorías únicas**: BEAUTY, BOOKS, CLOTHES, ELECTRONICS, FOOD, HOME, SPORT
- **Distribución por categoría principal**: 
  - ELECTRONICS: 5 usuarios
  - CLOTHES: 2 usuarios
  - HOME: 3 usuarios

## 🔍 Transformaciones Implementadas

### Ejemplo de Transformación
```python
# Antes de la limpieza
user_data = [' mike_reed ', 32.0]

# Después de la limpieza
user_data_clean = [['mike', 'reed'], 32]
```

### Impacto del Proyecto
- ✅ **100% de nombres normalizados** sin espacios innecesarios
- ✅ **100% de edades convertidas** de float a int
- ✅ **Separación exitosa** de nombres y apellidos
- ✅ **Preservación de integridad** en IDs, categorías y gastos

## 🚀 Cómo Replicar el Proyecto

### Clonar repositorio
```bash
git clone https://github.com/Baltazardv/limpieza-datos-usuarios.git
cd limpieza-datos-usuarios
```

### Ejecutar el notebook
```bash
# Opción 1: Jupyter Notebook
jupyter notebook proyecto_1_limpieza_datos_usuarios.ipynb

# Opción 2: JupyterLab
jupyter lab proyecto_1_limpieza_datos_usuarios.ipynb
```

### Estructura de Archivos
```
limpieza-datos-usuarios/
├── README.md
├── proyecto_1_limpieza_datos_usuarios.ipynb
└── reporte_datos_completo.md
```

## 🎯 Próximos Pasos

Este proyecto sienta las bases para:
1. **Análisis Exploratorio de Datos (EDA)** sobre categorías favoritas y comportamiento de compra
2. **Segmentación de clientes** por edad, preferencias y nivel de gasto
3. **Modelos predictivos** de valor de cliente (CLV)
4. **Automatización del proceso** con funciones para datasets más grandes
5. **Dashboard interactivo** para visualización de patrones de compra

## 💡 Habilidades Demostradas

- Limpieza y preparación de datos (Data Cleaning)
- Manipulación de strings en Python
- Conversión y validación de tipos de datos
- Análisis exploratorio básico
- Documentación técnica de procesos
- Pensamiento analítico para identificación de problemas de calidad

---

**📚 Proyecto desarrollado como parte del Bootcamp de Data Analytics en TripleTen**

**👨‍💻 Autor**: Baltazar Dimayuga  
**📧 Contacto**: [baltazardv13@gmail.com](mailto:baltazardv13@gmail.com)  
**💼 LinkedIn**: [linkedin.com/in/baltazar-dimayuga](https://linkedin.com/in/baltazar-dimayuga)  
**🐙 GitHub**: [github.com/Baltazardv](https://github.com/Baltazardv)
