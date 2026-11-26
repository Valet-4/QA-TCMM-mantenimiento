# Historias de usuario · QA-TCMM

Historias definidas para la Actividad 4 de Mantenimiento de Software (control de versiones con Git y GitHub).
Cada historia se implementa en su propia rama y se integra a `main` mediante un *pull request* que cierra el *issue* correspondiente.

| ID | Historia | Prioridad | Puntos | Rama | Estado |
|---|---|---|---|---|---|
| HU-01 | Cambiar entre tema claro y oscuro | Media | 2 | `feature/HU-01-tema-oscuro` | ✅ Implementada |
| HU-02 | Filtrar defectos por estado y severidad | Alta | 3 | `feature/HU-02-filtro-defectos` | ✅ Implementada |
| HU-03 | Comentar los defectos | Alta | 5 | `feature/HU-03-comentarios-defectos` | ✅ Implementada |
| HU-04 | Eliminar casos de prueba sin ejecuciones | Media | 3 | `feature/HU-04-eliminar-caso` | ⏳ Pendiente |
| HU-05 | Exportar los casos de prueba a CSV | Media | 2 | `feature/HU-05-exportar-casos` | ⏳ Pendiente |

## HU-01 · Cambiar entre tema claro y oscuro

**Como** analista QA o desarrollador, **quiero** cambiar manualmente entre el tema claro y el oscuro **para** trabajar cómodo durante jornadas largas sin depender de la configuración del sistema operativo.

**Criterios de aceptación**

- [x] En la barra lateral aparece el botón «Cambiar a modo oscuro» o «Cambiar a modo claro», según el tema activo.
- [x] Al pulsarlo, toda la interfaz cambia de tema de inmediato y se muestra un aviso de confirmación.
- [x] La preferencia se conserva al recargar la página o al volver a iniciar sesión.
- [x] Si el usuario nunca ha elegido un tema, se usa el del sistema operativo.

- Prioridad: Media · Estimación: 2 puntos
- Rama: `feature/HU-01-tema-oscuro` · Issue: #1
- Estado: Implementada

## HU-02 · Filtrar defectos por estado y severidad

**Como** analista QA, **quiero** filtrar la lista de defectos por estado y por severidad **para** encontrar rápido los defectos críticos o los que siguen abiertos.

**Criterios de aceptación**

- [x] El módulo Defectos tiene dos listas: Estado (Asignado, En corrección, Resuelto, Cerrado) y Severidad (Crítica, Alta, Media, Baja).
- [x] La tabla muestra solo los defectos que cumplen ambos filtros.
- [x] Se indica cuántos defectos se están mostrando del total («Mostrando X de Y»).
- [x] Si ningún defecto coincide, aparece un mensaje que lo explica.

- Prioridad: Alta · Estimación: 3 puntos
- Rama: `feature/HU-02-filtro-defectos` · Issue: #2
- Estado: Implementada

## HU-03 · Comentar los defectos

**Como** desarrollador, **quiero** dejar comentarios en un defecto y leer los del analista QA **para** comunicar avances, dudas o la causa encontrada sin salir de la plataforma.

**Criterios de aceptación**

- [x] Cada defecto tiene el botón «Comentarios (n)», donde n es la cantidad de comentarios.
- [x] La ventana de comentarios muestra autor, fecha y texto de cada comentario.
- [x] No se permite agregar un comentario vacío.
- [x] Al comentar, la otra parte (analista QA o desarrollador) recibe una notificación.

- Prioridad: Alta · Estimación: 5 puntos
- Rama: `feature/HU-03-comentarios-defectos` · Issue: #3
- Estado: Implementada

## HU-04 · Eliminar casos de prueba sin ejecuciones

**Como** analista QA, **quiero** eliminar un caso de prueba que creé por error y que aún no se ha ejecutado **para** mantener limpio el repositorio de casos sin perder la trazabilidad de los que ya se ejecutaron.

**Criterios de aceptación**

- [ ] El botón «Eliminar» solo aparece en los casos que no tienen ejecuciones registradas.
- [ ] Antes de eliminar se pide confirmación en una ventana.
- [ ] Al confirmar, el caso desaparece de la lista y de los indicadores, y se muestra un aviso.
- [ ] El perfil Desarrollador no puede eliminar casos.

- Prioridad: Media · Estimación: 3 puntos
- Rama: `feature/HU-04-eliminar-caso` · Issue: #4
- Estado: Pendiente

## HU-05 · Exportar los casos de prueba a CSV

**Como** líder de calidad, **quiero** descargar la lista de casos de prueba en un archivo CSV **para** compartirla con el equipo o abrirla en Excel.

**Criterios de aceptación**

- [ ] En el módulo Casos de prueba existe el botón «Exportar casos a CSV».
- [ ] El archivo incluye código, título, requisito, prioridad, estado, versión y pasos.
- [ ] Se exportan solo los casos visibles según la búsqueda y el filtro de estado.
- [ ] Las tildes se ven bien al abrir el archivo en Excel.

- Prioridad: Media · Estimación: 2 puntos
- Rama: `feature/HU-05-exportar-casos` · Issue: #5
- Estado: Pendiente
