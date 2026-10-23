# SupportDesk AI: Triage autónomo de tickets de soporte

Proyecto integrador del módulo 8. Un sistema que recibe tickets por Gmail,
los clasifica con IA, redacta una respuesta con una base de conocimiento,
pide aprobación humana en Slack y responde al cliente en el mismo hilo.

## Enlaces
- 📊 Dashboard de control: https://app.notion.com/p/Dashboard-de-Control-Triage-de-Soporte-IA-a6d1511a8d90453f9748ffa962813d6a?source=copy_link
- 🗄️ Base de datos (solo lectura): https://app.notion.com/p/Soporte-SaaS-Triage-3fe532b53b308041abf7cc94d0077085?source=copy_link

## Stack
| Categoría | Herramienta |
|---|---|
| Orquestador | n8n (local) |
| Base de datos | Notion |
| IA | Gemini Flash |
| Canales | Gmail y Slack |

## Contenido del repositorio
- `docs/arquitectura.pdf`: diagrama, esquema de tablas, JSON, matriz de costos y seguridad.
- `workflows/`: los dos workflows exportados (flujo principal y manejo de errores).
- `evidencias/`: capturas de los 8 casos de prueba, del esquema y del dashboard.

## Cómo importar los workflows
1. En n8n: **Workflows → Import from file**.
2. Crea tus propias credenciales (Gmail, Slack, Notion, Gemini) y asígnalas a los nodos.
3. Conecta las bases de Notion a tu integración y ajusta los IDs de las bases.

## Notas
Las credenciales no están incluidas. Los datos de prueba son ficticios.
