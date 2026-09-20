# AFL_AUTOS_HOME_UX_DEMO1

Demo pública experimental de la interfaz operativa AFL AUTOS.

## Objetivo

Validar una Home UX móvil/escritorio que permita operar dos frentes desde una sola pantalla:

1. estado y siguiente acción de vehículos;
2. seguimiento comercial de leads provenientes de Messenger y WhatsApp.

## Leads — Demo 1

La interfaz permite:

- registrar un lead;
- identificar canal `MESSENGER` o `WHATSAPP`;
- asociar vehículo de interés;
- registrar etapa comercial;
- programar fecha y hora del próximo seguimiento;
- registrar la próxima acción;
- distinguir vencidos, hoy y próximos;
- marcar contacto realizado;
- reprogramar;
- filtrar por canal y etapa;
- exportar/importar JSON para respaldo manual.

### Estados comerciales

```text
NUEVO
CONTACTADO
INFORMACION_ENVIADA
SEGUIMIENTO
CITA_PROGRAMADA
NEGOCIACION
GANADO
PERDIDO
PAUSADO
```

### Prioridad visual

```text
VENCIDO
→ HOY
→ PROXIMO
→ SIN_FECHA
→ CERRADO
```

## Flujo

```text
NUEVO MENSAJE
→ CREAR/IDENTIFICAR LEAD
→ DEFINIR SIGUIENTE ACCION
→ PROGRAMAR FECHA
→ CONTACTAR
→ REGISTRAR RESULTADO
→ REPROGRAMAR O CERRAR
```

## Persistencia

Demo 1 usa `localStorage` como cache temporal del navegador.

```text
localStorage = CACHE_DEMO
!=
FUENTE_DE_VERDAD
```

Permite exportar/importar JSON. Una versión productiva deberá conectarse con la fuente privada comercial vigente.

## Privacidad de esta prueba

Miguel autorizó probar una superficie pública con información privada para esta Demo 1.

Aun así, el repositorio no precarga PII real para evitar persistir accidentalmente nombres, teléfonos o conversaciones en GitHub. Los datos capturados desde la interfaz quedan en el navegador hasta que se exporten o eliminen.

## Archivos

- `index.html` — aplicación Demo 1.
- `docs/LEADS_UX.md` — diseño funcional del seguimiento comercial.

## Estado

```text
DEMO_1
CRM_LIGERO
MOBILE_FIRST
MESSENGER + WHATSAPP
PROGRAMACION_DE_SEGUIMIENTOS
NO_PRODUCTIVO
```
