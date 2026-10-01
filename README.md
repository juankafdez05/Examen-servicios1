# Dragon Ball · Net Warriors

Juego personal no oficial para repasar el examen de Servicios de Red.

Repositorio: `juankafdez05/Examen-servicios1`.

## Archivos

- `index.html`: juego completo, estilos, dibujos SVG, preguntas y guardado.
- `README.md`: instrucciones y limitaciones.

## Uso

Reemplazar completamente el `index.html` anterior por esta versión.

Puede abrirse como archivo local. No requiere instalación, bibliotecas,
imágenes remotas, fuentes externas ni conexión para sus recursos.

Después de actualizar una versión alojada, puede ser necesario recargar
sin caché para que el navegador utilice el archivo nuevo.

## Importante sobre acceso privado

El juego no incorpora autenticación.

Publicar un HTML sin una restricción de acceso real no garantiza que
solo su propietario pueda verlo. No se incluye una contraseña en
JavaScript porque no protegería realmente el contenido descargado.

Para uso estrictamente personal, puede ejecutarse localmente.

## Temática

Fan game educativo con:

- Goku, Vegeta y Gohan seleccionables.
- Nueve escenarios inspirados en Dragon Ball.
- Dibujos SVG simplificados originales.
- Ataques de ki y ataque especial.
- Guardia.
- Semillas senzu.
- Transformaciones visuales.
- Siete esferas y dos victorias finales.
- Jefes por saga.

No contiene imágenes, música ni logotipos oficiales descargados.
No está afiliado a los titulares de Dragon Ball.

Los nombres y escenarios se usan como ambientación.
El contenido evaluado es administración de sistemas y servicios de red.

## Mecánicas

### Modalidad A: reconocimiento

Cada objetivo tiene una pregunta con tres opciones, mezcladas en cada
intento. La corrección es automática.

### Modalidad B: explicación y aplicación

Hay que escribir una respuesta antes de revelar la solución.

Después se compara con tres criterios. La valoración es autoevaluada:
el juego no contiene una IA que interprete la respuesta.

Solo deben marcarse los criterios que la respuesta ya cumplía antes
de ver la solución.

### Vida

- Se empieza con cinco vidas.
- Un fallo resta una vida si no hay guardia.
- Un fallo vuelve a dejar pendiente esa modalidad.
- Al llegar a cero se vuelve al refugio.
- Se conserva el resto del progreso.
- Descansar restaura vida.
- Una senzu restaura hasta dos vidas.

### Ki y XP

- Primer acierto sin ayuda en una modalidad pendiente: 10 XP.
- Repetición correcta sin ayuda: 3 XP.
- Respuesta correcta con ayuda: 2 XP, sin acreditar.
- Acierto sin ayuda: 20 ki, hasta un máximo de 100.
- Acierto sin ayuda con 100 ki: ataque especial, consume el ki y añade 5 XP.
- Guardia: cuesta 30 ki y evita un daño, no un error.
- Primera victoria contra un jefe: 50 XP, una senzu y una vida.

La apariencia cambia a partir de 200 XP y de nuevo a partir de 650 XP.

### Ayudas

Una pista marca el intento como asistido.

Abrir el cuaderno durante un reto sin resolver también lo marca como
asistido. Ese intento no acredita la modalidad.

### Jefes

Para desbloquear un jefe se deben superar las dos modalidades de todos
los objetivos de su sala.

El jefe selecciona tres retos abiertos. Deben superarse los tres sin
ayuda.

Las victorias se conservan como logros históricos, aunque después se
falle una modalidad durante un repaso.

### Torneo mixto

18 retos: dos por sala, combinando reconocimiento y explicación.

El torneo es un repaso parcial, no sustituye el recorrido de los 52
objetivos.

## Cobertura académica

52 objetivos y 104 ejercicios base:

| Bloque | IDs | Objetivos |
|---|---|---:|
| SSH | S1–S7 | 7 |
| sudo | U1–U4 | 4 |
| Nombre del equipo | H1–H3 | 3 |
| Configuración de red | R1–R5 | 5 |
| Resolución de nombres | N1–N5 | 5 |
| Router y NAT | T1–T7 | 7 |
| DHCP | D1–D9 | 9 |
| Kea | K1–K8 | 8 |
| Diagnóstico | X1–X4 | 4 |
| **Total** | | **52** |

Fuentes académicas:

- Configuración inicial de un servidor Linux.
- Protocolo DHCP y servidor Kea.
- Guía del examen facilitada por el usuario.

Las referencias aparecen en cada explicación.

Las situaciones compuestas a partir de conceptos de los apuntes se
identifican como aplicaciones razonadas, no como prácticas observadas.

No se ha utilizado la investigación visual sobre Dragon Ball para
ampliar el contenido académico.

## Siete objetivos con cobertura documental parcial

Los PDF disponibles no desarrollan todos los detalles exigidos:

| ID | Material que falta |
|---|---|
| S7 | Reenvío del agente y práctica de ssh -A |
| D2 | Condiciones broadcast/unicast de todos los mensajes DORA |
| K6 | Sintaxis y condiciones de reservas Kea |
| K8 | Captura real y uso de tcpdump |
| X1 | Comprobaciones específicas en Linux y Windows al apagar DHCP |
| X2 | Práctica sobre cambios con concesiones activas |
| X3 | Corrección persistente de rutas por defecto duplicadas |

Estos puntos no se ocultan ni se consideran completamente cubiertos
por superar sus ejercicios.

La aplicación distingue:

1. Modalidades practicadas: máximo 104.
2. Objetivos con ambas modalidades y sin laguna: máximo 45 con este banco.

Para alcanzar una cobertura documental completa se deben incorporar
las prácticas que faltan y revisar las preguntas correspondientes.

## Guardado

Se utiliza la misma clave que en la versión anterior:

    rootquest-servicios1-v1

Se intenta recuperar el progreso anterior si se abre desde el mismo
navegador y origen.

El guardado incluye:

- Vida, XP, ki, racha y senzu.
- Personaje.
- Modalidades superadas.
- Intentos y errores.
- Jefes vencidos.
- Última sala.
- Sonido.
- Hasta 200 resultados recientes.

No incluye los textos de las respuestas abiertas.

No se sincroniza con GitHub ni se envía a un servidor.

Exportar una copia antes de cambiar de navegador, dispositivo o
ubicación del archivo.

## Herramientas

Desde Partida:

- Exportar progreso como JSON.
- Importar progreso con validación.
- Exportar cobertura como Markdown.
- Cambiar personaje.
- Activar sonido.
- Reiniciar progreso con confirmación.

## Validaciones incluidas

Al arrancar se comprueba:

- 52 objetivos.
- IDs únicos.
- Distribución correcta entre salas.
- Tres criterios por respuesta abierta.
- Pregunta, respuesta y explicación presentes.
- Opciones sin duplicados dentro de cada pregunta.
- Siete objetivos parciales identificados.

Estas validaciones no sustituyen las pruebas de ejecución de la interfaz.

El código no se ejecutó en un navegador durante su entrega en la
conversación.

## Si no arranca

Hay un bloque de diagnóstico independiente del motor del juego.

Si se produce un error de JavaScript, intenta mostrar:

- Mensaje.
- Número de línea.

Si la página sigue mostrando solamente “Preparando el radar”, revisar
la consola del navegador y confirmar que se ha copiado el archivo
completo, incluidos los dos bloques de script y el cierre de HTML.

## Pruebas manuales recomendadas

- [ ] Aparecen las nueve sagas.
- [ ] El temario muestra 52 objetivos.
- [ ] Se indican siete objetivos parciales.
- [ ] Un acierto muestra explicación, XP y ataque.
- [ ] Un error muestra explicación y resta vida.
- [ ] La guardia consume ki y evita daño, pero no acredita el fallo.
- [ ] Una senzu restaura vida.
- [ ] Una pista impide acreditar el intento.
- [ ] El cuaderno marca el intento como asistido.
- [ ] Una respuesta abierta requiere comparación con criterios.
- [ ] No se puede puntuar dos veces el mismo intento.
- [ ] Los jefes se desbloquean tras completar la sala.
- [ ] Llegar a cero vidas permite recuperarse.
- [ ] La recarga conserva progreso cuando el navegador permite guardarlo.
- [ ] Exportar e importar funciona.
- [ ] Se rechaza un JSON inválido.
- [ ] La interfaz se puede usar con teclado y en móvil.

## Objetivo del proyecto

La ambientación motiva el repaso.
El objetivo real es poder explicar, configurar y comprobar los servicios
sin depender de respuestas de opción múltiple.
