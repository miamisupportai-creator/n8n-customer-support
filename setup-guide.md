# Guia de Setup — AI Customer Support Bot

## Descripcion
Bot de soporte con IA (Claude) vía webhook. Clasifica el intent del mensaje automaticamente y genera respuestas personalizadas en segundos.

## Pasos
1. Importar `workflow.json` en n8n
2. Crear credencial Anthropic API (Header Auth) en Settings > Credentials
3. Reemplazar `${CLIENT_ID}` en el nodo "AI Response" con el API key de Anthropic
4. Conectar tu canal (WhatsApp, web chat, email) al webhook
5. Activar y testear

## Variables Configuradas
| Variable | Valor |
|----------|-------|
| CLIENT_ID | ${CLIENT_ID} |
| CLIENT_NAME | ${CLIENT_NAME} |
| CLIENT_PHONE | ${CLIENT_PHONE} |

## Webhook URL
`https://ai50m.app.n8n.cloud/webhook/support-${CLIENT_ID}`

## Intents Detectados
| Intent | Palabras Clave |
|--------|---------------|
| pricing | precio, costo, price |
| cancellation | cancelar, cancel |
| technical | problema, error, no funciona |
| scheduling | hora, horario, cita |
| general | todo lo demas |

## Soporte
contact@ai50m.com | ai50m.com
