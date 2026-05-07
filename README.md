# 📊 JoinTech - Database Project

## 🏢 Sobre el proyecto

Este proyecto forma parte del desarrollo de la base de datos de **JoinTech**, una empresa orientada a la gestión de productos, pedidos y experiencia de usuario en un entorno e-commerce.

El objetivo principal es diseñar, implementar y analizar una base de datos relacional optimizada para la gestión de operaciones comerciales.

---

## 🗂️ Estructura de la Base de Datos

La base de datos de JoinTech está compuesta por las siguientes tablas:

### 📁 Tablas principales

* **categories** → Clasificación de productos
* **products** → Información de los productos
* **orders** → Pedidos realizados por los clientes
* **order_items** → Detalle de los productos dentro de cada pedido
* **payments** → Información de los pagos
* **reviews** → Opiniones y valoraciones de los clientes

---

## 🔗 Relaciones entre tablas

* Un **producto** pertenece a una **categoría**
* Un **pedido** puede contener múltiples **productos** (relación a través de `order_items`)
* Un **pedido** tiene asociado un **pago**
* Un **producto** puede tener múltiples **reviews**

---

## 🧱 Modelo lógico simplificado

```
categories
    ↓
products
    ↓
order_items ← orders → payments ó → customers
    ↓
reviews
```

---

## ⚙️ Tecnologías utilizadas

* SQL (BigQuery compatible)
* Python (para carga y manipulación de datos)
* Google Cloud BigQuery
* Git & GitHub para control de versiones

---

## 🚀 Objetivos del proyecto

* Diseñar un modelo relacional eficiente
* Garantizar integridad referencial
* Permitir análisis de negocio mediante SQL
* Optimizar consultas para grandes volúmenes de datos

---

## 📊 Ejemplos de análisis

Algunos análisis que permite esta base de datos:

* Productos más vendidos
* Ingresos por categoría
* Clientes con mayor gasto
* Valoraciones medias por producto
* Tasa de conversión de pedidos

---

## 📌 Buenas prácticas aplicadas

* Normalización de datos (hasta 3FN)
* Uso de claves primarias
* Separación de entidades (orders vs order_items)
* Diseño escalable

---

## 🧪 Cómo usar el proyecto

1. Clonar el repositorio:

```bash
git clone <repo-url>
```

2. Configurar entorno virtual:

```bash
python -m venv venv
source venv/bin/activate
```

3. Instalar dependencias:

```bash
pip install -r requirements.txt
```

4. Configurar credenciales en `.env`

5. Ejecutar scripts o notebooks para crear tablas y cargar datos

---

## 👥 Equipo

Proyecto desarrollado por:

    **SRCUM MASTER**: Maksym Chaika Palamaryuk
    **Data Modeler**: Daniel García Ordiales
    **Data Engineer**: Pablo Hernández Hernández
    **QA/Docs**: Ana Belen Balmaseda Afqir

---

## 📄 Licencia

Este proyecto es de uso educativo y demostrativo.
