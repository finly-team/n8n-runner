# n8n-runner (Task Runners sidecar)

## Requisitos
- La versión del runner debe coincidir con la versión de n8n (ej: 2.1.5).
- El servicio n8n debe tener habilitado external task runners.

## Variables de entorno (en este servicio runner)
- N8N_RUNNERS_AUTH_TOKEN=<igual al de n8n>
- N8N_RUNNERS_TASK_BROKER_URI=http://<HOST_INTERNO_N8N>:5679
- N8N_RUNNERS_AUTO_SHUTDOWN_TIMEOUT=15
- (opcional) N8N_RUNNERS_LAUNCHER_LOG_LEVEL=debug

## Nota
No es necesario exponer puertos públicamente para el runner.
Debe estar en el mismo proyecto/red que el servicio n8n para que resuelva el hostname interno.
