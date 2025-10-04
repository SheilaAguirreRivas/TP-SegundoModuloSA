# TP-SegundoModuloSA
TRABAJO PRÁCTICO - Segundo Módulo de Programación Avanzada para Ciencia de Datos
# Análisis de Medicamentos GAVADE

## 📌 Descripción
Este proyecto corresponde al Trabajo Práctico sobre Módulo 2.  
Se trabaja con el dataset **GAVADE**, que contiene información sobre medicamentos, precios de referencia (PVP PAMI), cobertura y el importe que abonan los afiliados.

https://datos.gob.ar/dataset/pami-listado-precios-medicamentos-para-entidades/archivo/pami_e72a9026-a971-46c1-b828-2638b2b2be37

El objetivo es:
1. Obtener y limpiar el dataset.
2. Almacenarlo en una base de datos SQL Server.
3. Construir un dashboard en Google Colab para analizar la información.
   
https://colab.research.google.com/drive/1_C4Ek1tNZSnNo1LGZ9SbojHC-Sxyc4I1#scrollTo=g8e4c-rtNMIb 


⚙️ Configuración del motor de base de datos (SQL Server)

1 Instalación de SQL Server

Descargar e instalar SQL Server (Developer o Express edition).

Instalar también SQL Server Management Studio (SSMS) para administrar la base de datos gráficamente.

2 Creación de la base de datos

Crear una nueva base de datos llamada, por ejemplo:

CREATE DATABASE medic;


Seleccionarla para trabajar:

USE medic;


3 Creación de la tabla gavade
Se puede crear una tabla que refleje la estructura de los datos cargados en el análisis de Colab

CREATE TABLE dbo.Vademecum_20251001_091834 (
    ALFABETA FLOAT NULL,
    [PRINCIPIO ACTIVO] NVARCHAR(255) NULL,
    [MARCA COMERCIAL] NVARCHAR(255) NULL,
    PRESENTACION NVARCHAR(255) NULL,
    LABORATORIO NVARCHAR(255) NULL,
    [PVP PAMI AL 01/10/2025] NVARCHAR(255) NULL,
    COBERTURA NVARCHAR(255) NULL,
    [IMPORTE AFILIADO] NVARCHAR(255) NULL
);

4 Carga de datos

Importar el archivo Excel directamente desde SSMS con la opción Import Data.
---

## ⚙️ Requisitos
- Python 3
- Librerías:
  - pandas
  - plotly
  - sqlalchemy
  - openpyxl
  - statsmodels (para la recta de tendencia)

---

## 🚀 Ejecución
1. Clonar este repositorio:
   ```bash
   git clone <URL_DEL_REPO>
