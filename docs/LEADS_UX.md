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
