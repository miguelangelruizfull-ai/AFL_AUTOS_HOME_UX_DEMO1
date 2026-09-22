# AFL_AUTOS_HOME_UX_DEMO1

Demo pública experimental de la interfaz operativa AFL AUTOS.

## Estado actual

```text
DEMO_2
HOME_OPERATIVA_UNIFICADA
MOBILE_FIRST + DESKTOP
LEADS + VEHICULOS + PRODUCCION + RECURSOS + ROOT + LAB
NO_PRODUCTIVO
```

## Objetivo

Validar una sola interfaz para operar, sin depender de abrir múltiples HTML o recordar prompts/rutas para tareas cotidianas.

La navegación de Demo 2 incorpora:

- Inicio / centro de trabajo;
- Operaciones;
- Respuestas y seguimiento de leads;
- ficha de vehículo y editor JSON local;
- retorno a producción manual;
- Drive / GitHub como accesos configurables localmente;
- ROOT Console como vista de coordinación;
- AFL Autos Lab para pruebas.

## Privacidad

Este repositorio es público. Por diseño:

- no precarga PII real;
- no contiene conversaciones reales;
- no hardcodea enlaces privados de Drive;
- no hardcodea repositorios privados;
- no convierte `localStorage` en fuente de verdad;
- los enlaces privados que el usuario configure desde la UI se guardan únicamente en el navegador;
- la exportación de respaldo de Demo 2 no incluye los valores de esos enlaces privados, solo sus nombres configurados.

## Persistencia

```text
localStorage = CACHE_DEMO
!=
FUENTE_DE_VERDAD
```

Demo 2 reutiliza la clave de leads de Demo 1 para no perder la prueba local previa y agrega almacenamiento local separado para vehículos demo, enlaces privados y retorno de producción.

## Arquitectura UX

```text
HOME UX
├─ INICIO
├─ OPERACIONES
├─ RESPUESTAS / LEADS
├─ VEHICULOS
├─ PRODUCCION MANUAL
├─ DRIVE / GITHUB
├─ ROOT CONSOLE
└─ AFL AUTOS LAB
```

La Home es interfaz; las fuentes de verdad siguen perteneciendo a los repositorios y almacenamientos autorizados de cada frente.

## Siguiente fase productiva

```text
HOME UX
→ CAPA PRIVADA AUTENTICADA
→ FUENTE COMERCIAL PRIVADA
→ FUENTES DE VEHICULOS / OPERACION
→ ACCIONES CONTROLADAS
→ EXPORTACION SANITIZADA
```

La integración productiva requiere autenticación y conectores o APIs autorizadas. No debe resolverse publicando datos privados en GitHub.
