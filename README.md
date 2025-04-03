# 📊 Generador de Reportes Bera Motorcycles

Aplicación desarrollada en **Streamlit** que permite generar y descargar reportes contables desde una base de datos PostgreSQL alojada en Azure, basada en tres flujos principales:

- 🔍 **Placas por Cliente (CINTAS)** – Consulta por número de cinta.
- 📑 **Facturación con Seriales (SENIAT)** – Consulta por fecha y localidad.
- 📦 **Despachos (SENIAT)** – Consulta por fecha de despacho y localidad.

---

## 🚀 Instalación

1. Clona este repositorio:

```bash
git clone https://github.com/tu_usuario/streamlit-reportes-bera.git
cd streamlit-reportes-bera
```

2. Instala las dependencias:

```bash
pip install -r requirements.txt
```

3. Crea el archivo `.env` en la raíz del proyecto con tu configuración de base de datos:


> ⚠️ **Importante:** El archivo `.env` está en `.gitignore` para evitar exponer credenciales.

---

## ▶️ Ejecución

Lanza la aplicación localmente:

```bash
streamlit run app.py
```

Esto abrirá una interfaz web interactiva donde podrás:

- Seleccionar el tipo de reporte.
- Ingresar los parámetros requeridos (fecha, localidad, cinta).
- Visualizar los datos en tabla.
- Descargar un archivo Excel con el nombre dinámico adecuado.

---

## 📂 Estructura del Proyecto

```
📁 streamlit-reportes-bera/
├── app.py
├── .env            # NO se sube al repositorio
├── requirements.txt
└── README.md
```

---

## ✅ Dependencias principales

- [Streamlit](https://streamlit.io)
- Pandas
- Psycopg2
- OpenPyXL
- python-dotenv

---

## 🔐 Seguridad

Este proyecto utiliza un archivo `.env` para mantener las credenciales de la base de datos fuera del repositorio. Nunca subas este archivo a GitHub.

---

## 🧠 Autor

Desarrollado por Hidelberg Martínez   
Trabajo realizado para **Bera Motorcycles** – Departamento de Sistemas.