# UX — LEADS MESSENGER + WHATSAPP

## Necesidad agregada

La Home no debe limitarse a producción/contenido.

Debe ayudar a responder:

1. ¿A quién tengo que contactar hoy?
2. ¿Qué seguimientos están vencidos?
3. ¿Qué cliente está esperando información?
4. ¿Qué vehículo le interesa?
5. ¿Cuál es la próxima acción?
6. ¿Cuándo debo volver a escribirle?
7. ¿De qué canal viene: Messenger o WhatsApp?

## Entidad LEAD

Campos mínimos:

- nombre o alias;
- canal;
- referencia de contacto;
- vehículo de interés;
- etapa;
- prioridad;
- fecha/hora de próximo seguimiento;
- última interacción;
- próxima acción;
- notas;
- resultado;
- creado;
- actualizado.

## UX móvil

La pantalla inicial muestra:

- VENCIDOS;
- HOY;
- PRÓXIMOS;
- SIN FECHA;
- botón `+ LEAD`;
- lista ordenada por urgencia;
- acción rápida `CONTACTAR`;
- acción rápida `REPROGRAMAR`.

## UX escritorio

Además:

- columna de filtros;
- lista central de leads;
- panel contextual derecho con detalle y próxima acción.

## Regla operativa

```text
NUEVO MENSAJE
→ CREAR/IDENTIFICAR LEAD
→ DEFINIR SIGUIENTE ACCION
→ PROGRAMAR FECHA
→ CONTACTAR
→ REGISTRAR RESULTADO
→ REPROGRAMAR O CERRAR
```

## Próxima fase productiva

Conectar la UI con la fuente privada comercial vigente, manteniendo GitHub público como frontend/demo y sin convertir JSON público en maestro.


## Iteración autorizada — Agenda operativa

Se agregó:

- resumen de agenda al abrir la Home;
- prioridad visual para vencidos y seguimientos de hoy;
- botón `REPROGRAMAR` por lead;
- atajos `HOY +2H`, `MAÑANA 10:00`, `+3 DÍAS`, `+7 DÍAS`;
- exportación individual a calendario mediante `.ics`;
- botón `ABRIR DETALLE` separado de acciones rápidas.

Objetivo UX:

```text
VER PRIORIDAD
→ CONTACTAR
→ REGISTRAR RESULTADO
→ REPROGRAMAR
→ CALENDARIO
```

La agenda de la demo sigue siendo local al navegador y no reemplaza una agenda o CRM productivo.
