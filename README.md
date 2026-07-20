# FPM – Asistente Comercial IA

Proyecto final del curso Ecosistema de Automatización IA Autónomo para Negocios.

## Descripción

Sistema de automatización comercial para FPM S.A. que recibe consultas, interpreta lenguaje natural con inteligencia artificial, busca coincidencias en un catálogo de productos y genera una respuesta propuesta.

Antes de contactar al cliente, la respuesta debe ser aprobada por una persona mediante una interfaz de Airtable.

## Tecnologías utilizadas

- n8n
- Airtable
- OpenAI
- Gmail

## Funcionamiento

1. La consulta ingresa mediante un formulario de Airtable.
2. Airtable registra la información.
3. n8n procesa el mensaje con OpenAI.
4. La IA clasifica la consulta y extrae códigos y datos técnicos.
5. El sistema busca coincidencias en la tabla Productos.
6. Airtable registra los resultados.
7. Gmail notifica al responsable comercial.
8. La respuesta queda pendiente de aprobación humana.
9. Si es aprobada, Gmail envía la respuesta final al cliente.
10. Si es rechazada, queda en estado Requiere corrección.

## Human-in-the-loop

El sistema no envía una respuesta comercial final sin una aprobación humana explícita.

## Pruebas realizadas

- Producto encontrado.
- Producto no encontrado.
- Datos faltantes.
- Notificación al responsable.
- Consulta aprobada.
- Consulta rechazada.
- Envío final al cliente.
- Camino infeliz.

## Estructura del repositorio

- `docs/`: documentación y diagrama de arquitectura.
- `workflows/`: archivos JSON exportados desde n8n.
- `screenshots/`: evidencias del funcionamiento.
- `links/`: enlaces públicos de Airtable y video.

## Documentación

El documento completo se encuentra en:

`docs/arquitectura-fpm-asistente-comercial-ia.pdf`

## Enlaces

Los enlaces públicos se encuentran en:

`links/enlaces-demo.md`

## Autor

Gonzalo Raffaele
