# GA4-API-PYTHON

```markdown
# API Google Analytics - Informe y Gráficos

Este es un script de Python que se conecta a la API de Google Analytics, obtiene datos y genera informes y gráficos.

## Requisitos

Asegúrate de tener las siguientes bibliotecas de Python instaladas:

- Pandas
- Matplotlib
- Otras bibliotecas necesarias para tu proyecto (como google-auth, google-auth-oauthlib, google-auth-httplib2, etc.)

Puedes instalar estas bibliotecas utilizando `pip`:

```bash
pip install pandas matplotlib google-auth google-auth-oauthlib google-auth-httplib2
```

## Uso

1. Define las credenciales de la API de Google Analytics en un archivo JSON y configura la variable de entorno `GOOGLE_APPLICATION_CREDENTIALS` para que apunte a ese archivo.

2. Ejecuta el script proporcionando la fecha de finalización y el número de días de datos que deseas obtener:

```python
produce_report(end_date, no_days)
```

Esto generará un informe y gráficos basados en los datos de Google Analytics para el período especificado.

## Funcionalidad

- El script utiliza la API de Google Analytics para obtener datos.

- Calcula la fecha de inicio en función de la fecha de finalización y el número de días especificados.

- Genera un informe con datos de tráfico diario, usuarios activos por página y usuarios activos por página de destino.

- Crea gráficos de pastel y gráficos de líneas para visualizar los datos.

- Muestra las 10 principales páginas de destino y las 10 principales páginas visitadas en forma de tablas.

## Problemas conocidos

- Puede haber problemas con la hashabilidad de los nombres de columna en los DataFrames de Pandas. Asegúrate de que los nombres de las columnas sean hashables o realiza la conversión necesaria.

- Otros problemas relacionados con la configuración de la API de Google Analytics o el entorno de Python pueden surgir y deben resolverse según sea necesario.

¡Disfruta utilizando este script para generar informes y gráficos a partir de los datos de Google Analytics!
```

Este archivo `README.md` proporciona una descripción general de tu código, los requisitos necesarios, cómo utilizarlo y algunos problemas conocidos. Puedes personalizarlo y agregar más detalles según sea necesario para tu proyecto.
