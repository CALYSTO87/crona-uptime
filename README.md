# crona-uptime

Alerta externa de caídas de Crona. Un workflow programado de GitHub Actions pide `https://crona.com.ar/api/health`
cada 10 minutos y, si no responde 200, abre un issue con la etiqueta `caida`. El issue se cierra solo cuando vuelve.

Es público para no consumir minutos de Actions. No tiene secretos: sólo consulta un endpoint público.
