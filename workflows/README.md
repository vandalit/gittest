# Workflows de n8n

En esta carpeta se almacenan las exportaciones en formato JSON de los workflows construidos para este proyecto:

1. `alerta-lluvia.json`: Consulta pronóstico horario vía Open-Meteo API, evalúa probabilidad de lluvia en las próximas 24 horas y notifica por Discord/Telegram.
2. `alerta-sismo.json`: Consulta sismos recientes vía USGS Earthquake API, filtra eventos locales en una ventana de 15-20 minutos y notifica si superan la magnitud configurada.

### Cómo importarlos en n8n:
1. Abre tu interfaz de n8n en el navegador (`http://localhost:5678`).
2. Haz clic en **Workflows** > **Add workflow** (o botón `+`).
3. En el menú superior derecho (tres puntos `...`), selecciona **Import from File** y elige el archivo `.json` correspondiente.
