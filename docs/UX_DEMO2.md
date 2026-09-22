# UX DEMO 2 — HOME OPERATIVA UNIFICADA

## Problema que resuelve

Demo 1 validó seguimiento de leads, pero la navegación inferior todavía no resolvía una operación completa. Demo 2 convierte la Home en una consola de trabajo única.

## Principio

```text
ENTRAR POR TAREA
NO POR ARCHIVO
```

El usuario debe poder abrir la Home y responder:

1. ¿qué está vencido?;
2. ¿a quién debo contactar?;
3. ¿qué vehículo estoy trabajando?;
4. ¿qué atributos tiene?;
5. ¿a qué etapa de producción quiero regresar?;
6. ¿dónde están mis recursos?;
7. ¿cómo regreso a ROOT o al LAB?

## Navegación

### Móvil

Barra inferior:

```text
INICIO | LEADS | AUTOS | PRODUCIR | MAS
```

### Escritorio

Sidebar persistente:

```text
Inicio
Operaciones
Respuestas / Leads
Vehículos
Producción
Drive / GitHub
ROOT Console
AFL Autos Lab
```

## Frontera de privacidad

La Demo 2 NO escribe enlaces privados dentro del HTML. Los accesos se configuran en el navegador y quedan en `localStorage`.

La exportación general omite los valores de enlaces privados.

## Producción manual

El módulo de producción no ejecuta prompts ni muta repositorios/Drive. Registra una intención local con vehículo, etapa y objetivo para validar la UX.

## Próximo gate

Antes de ejecutar acciones reales desde la interfaz se requiere una capa privada autenticada y contratos claros por módulo.
