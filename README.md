# ROOT QUEST — Examen de Servicios

Juego de repaso para el repositorio `juankafdez05/Examen-servicios1`.

## Inicio rápido

1. Guarda el código del juego en `index.html`.
2. Guarda este documento en `README.md`.
3. Abre `index.html` en un navegador moderno.
4. Entra en una sala y empieza por el siguiente terminal.

No requiere instalación, dependencias, CDN, fuentes externas ni servidor
para el uso local. No ejecuta comandos del sistema: todos los ejercicios
son simulaciones educativas.

## Archivos

    Examen-servicios1/
    ├── index.html
    └── README.md

## Privacidad: importante

El HTML no incluye autenticación ni control de acceso.

- Usar el archivo localmente evita tener que publicar el juego.
- Subirlo a un repositorio y publicarlo como web son acciones distintas.
- No debe suponerse que una web es privada por el nombre del repositorio
  o porque nadie conozca su dirección.
- Una contraseña incluida en JavaScript no sería una protección real
  del contenido descargado.
- Para acceso exclusivamente personal en línea, el alojamiento debe
  imponer una restricción de acceso real antes de servir el contenido.

No se incluyen instrucciones para publicar una web abierta porque el
requisito indicado es que solo el propietario pueda acceder.

El código del juego no hace peticiones de red, no incorpora analítica
y no utiliza servicios de terceros.

## Mecánicas

### Nueve salas

1. Bastión SSH
2. Fortaleza sudo
3. Archivo de Identidades
4. Sala de Interfaces
5. Laberinto NSS
6. Frontera NAT
7. Torre DHCP
8. Motor Kea
9. Sala del Reinicio

Cada sala contiene terminales y un jefe.

### Dos modalidades por objetivo

**A. Reconocimiento**

Pregunta con tres opciones. El orden se mezcla en cada intento.

**B. Explicación y aplicación**

Caso abierto que exige redactar una respuesta antes de mostrar la
solución. Después se compara con tres criterios.

La corrección abierta es AUTOEVALUADA. No hay una IA analizando la
respuesta ni un corrector semántico disfrazado de evaluación automática.

Marcar criterios que no estaban en la respuesta elimina el valor del
repaso. Sé exigente: el objetivo es aprender, no ganar puntos.

### Vida y experiencia

- Empiezas con cinco vidas.
- Un fallo resta una vida.
- El error deja pendiente la modalidad correspondiente.
- Los fallos se registran en el cuaderno.
- Con cero vidas vuelves al refugio.
- Conservas XP, jefes vencidos y el resto del aprendizaje.
- Puedes descansar sin penalización de tiempo.
- Una poción restaura hasta dos vidas.

Puntuación:

- Primera superación sin pista de una modalidad pendiente: 10 XP.
- Repetición correcta ya acreditada: 3 XP.
- Respuesta correcta con pista: 3 XP, sin acreditar la modalidad.
- Primera victoria contra un jefe: 50 XP, una poción y una vida.

### Jefes

Se desbloquean al superar las dos modalidades de todos los terminales
de su sala.

Cada jefe selecciona tres retos abiertos de esa sala.
Hay que superar los tres sin pistas.

Los jefes no son una prueba independiente de corrección automática:
sus respuestas abiertas también son autoevaluadas.

### Animaciones

- Ataque del administrador.
- Impacto sobre el enemigo.
- Retroceso y daño al fallar.
- Pérdida de vida visible.
- Movimiento del personaje según el avance en la sala.
- Confeti al completar hitos.
- Sonidos opcionales.

Se respeta `prefers-reduced-motion`.

## Modos adicionales

### Repaso de errores

Selecciona hasta diez objetivos con errores y modalidades pendientes.
Prioriza los que acumulan más fallos.

### Simulacro mixto

Selecciona dos objetivos de cada sala: 18 retos en total.
Combina reconocimiento y explicación.

No reemplaza el recorrido completo de los 52 objetivos.

### Cuaderno

Permite revisar soluciones, fuentes, rúbricas y lagunas documentales.
Leer una solución no acredita una modalidad.

### Matriz de cobertura

Muestra los 52 objetivos con:

- ID.
- Nombre.
- Estado de reconocimiento.
- Estado de explicación.
- Variante práctica.
- Fuente.
- Laguna documental, si existe.

Se puede buscar y exportar como Markdown.

## Fuentes y límites

El contenido académico procede de:

1. Configuración inicial de un servidor Linux.
2. Protocolo DHCP y servidor Kea.
3. Guía del examen facilitada por el usuario.

Las referencias a diapositivas están incluidas en el juego.

Los casos nuevos se identifican como aplicación razonada cuando combinan
conceptos de los apuntes. No deben confundirse con resultados observados
en una práctica real.

No se han consultado fuentes externas para ampliar el temario.

### Advertencia sobre cobertura

Se han registrado los 52 puntos de la guía, sin omitir categorías.
Eso NO significa que los PDF disponibles desarrollen todos sus detalles.

Hay 8 objetivos con cobertura documental parcial:

| ID | Parte que falta desarrollar |
|---|---|
| S7 | Reenvío del agente y secuencia práctica de `ssh -A` |
| D2 | Broadcast/unicast de todos los mensajes DORA y sus condiciones |
| K6 | Sintaxis y condiciones de configuración de reservas Kea |
| K8 | Comando, filtro e interpretación de captura real con `tcpdump` |
| X1 | Comprobaciones concretas en Linux y Windows al apagar DHCP |
| X2 | Procedimiento y resultados ante cambios con concesiones activas |
| X3 | Corrección persistente de rutas por defecto duplicadas |
| X4 | No tiene laguna marcada: se plantea como lista de comprobación razonada |

**Corrección del recuento de la tabla:** X4 es una aclaración, no un
objetivo parcial. Los objetivos marcados con laguna en el banco son
**S7, D2, K6, K8, X1, X2 y X3: 7 en total**.

El contador de la aplicación se calcula directamente del banco y
muestra esos 7 objetivos parciales.

Se incluyen ejercicios sobre las partes justificables, pero se señala
lo que falta. Un objetivo con laguna no pasa a considerarse totalmente
cubierto por acertar el ejercicio.

Para completar estos apartados se necesita la práctica correspondiente
o apuntes adicionales. No se han inventado soluciones y atribuido al PDF.

### Interpretación del progreso

Hay dos indicadores distintos:

1. **Práctica:** modalidades superadas de un total de 104.
2. **Objetivos sin laguna documental y con ambas modalidades superadas.**

Con el banco actual, el segundo indicador no puede alcanzar 52/52:
los siete objetivos parciales siguen pendientes de material.

Completar nueve jefes tampoco demuestra que se haya realizado una
práctica real sobre máquinas Linux y Windows.

## Inventario de objetivos

| Sala | IDs | Cantidad |
|---|---|---:|
| SSH | S1–S7 | 7 |
| sudo | U1–U4 | 4 |
| Nombre del equipo | H1–H3 | 3 |
| Red | R1–R5 | 5 |
| Resolución de nombres | N1–N5 | 5 |
| Router y NAT | T1–T7 | 7 |
| DHCP | D1–D9 | 9 |
| Kea | K1–K8 | 8 |
| Comprobación y razonamiento | X1–X4 | 4 |
| **Total** | | **52** |

### SSH

- S1: simétrico frente a asimétrico.
- S2: firma y reto.
- S3: autenticación paso a paso.
- S4: ubicación de claves.
- S5: claves frente a contraseñas.
- S6: ssh-keygen y ssh-copy-id.
- S7: salto por router y ssh -A.

### sudo

- U1: root, mínimo privilegio, auditoría y control.
- U2: sudoers, sudoers.d y visudo.
- U3: NOPASSWD.
- U4: comprobación con sudo -k.

### Nombre del equipo

- H1: hostname y FQDN.
- H2: hostname y hosts.
- H3: hostnamectl y comprobaciones.

### Red

- R1: interfaz, IP, máscara, gateway y DNS.
- R2: estático frente a dinámico.
- R3: gestores y ubicaciones.
- R4: configuración persistente estática y DHCP.
- R5: consulta de configuración activa.

### Resolución

- N1: NSS y hosts:.
- N2: hosts frente a resolv.conf.
- N3: systemd-resolved.
- N4: DNS directo frente a NSS.
- N5: resolución estática aplicada.

### Router

- T1: forwarding persistente.
- T2: SNAT frente a DNAT.
- T3: MASQUERADE.
- T4: iptables-nft.
- T5: construcción de reglas.
- T6: persistencia y arranque.
- T7: entrada exterior por el router.

### DHCP

- D1: finalidad y puertos.
- D2: DORA y difusión.
- D3: REQUEST y ACK con varios servidores.
- D4: estados.
- D5: T1, T2 y T3.
- D6: renovación y respuestas.
- D7: INIT-REBOOT.
- D8: ámbito, rango, concesión y reserva.
- D9: parámetros enviados.

### Kea

- K1: servicios y archivos.
- K2: estructura de configuración.
- K3: subred frente a pool.
- K4: ámbito completo.
- K5: varios ámbitos.
- K6: reserva y DNAT.
- K7: concesiones y registros.
- K8: captura e identificación.

### Diagnóstico

- X1: apagar DHCP.
- X2: cambiar configuración con concesión activa.
- X3: interfaz pública y ruta por defecto.
- X4: comprobación después del reinicio.

## Guardado

Clave local:

    rootquest-servicios1-v1

La partida se guarda en localStorage cuando el navegador lo permite.

Incluye:

- Vidas.
- XP.
- Pociones.
- Modalidades superadas.
- Intentos y errores.
- Jefes vencidos.
- Última sala.
- Preferencia de sonido.
- Hasta 200 resultados recientes.

No guarda los textos de las respuestas abiertas.

El guardado depende del navegador y del origen desde el que se abre el
archivo. No se promete que una partida abierta como archivo local se
comparta con una versión alojada ni con otro navegador.

Exporta una copia antes de cambiar de equipo o ubicación.

### Exportación e importación

Desde Partida:

- Exportar partida: descarga un JSON.
- Importar partida: valida el JSON antes de sustituir el progreso.
- Exportar matriz: descarga un resumen de cobertura en Markdown.
- Reiniciar: solicita confirmación.

El archivo de progreso es editable por su propietario.
No está diseñado como sistema antifraude ni como calificación oficial.

## Verificación incluida

Al cargar, el código comprueba:

- Exactamente 52 objetivos.
- IDs únicos.
- Distribución correcta por salas.
- Pregunta y variante presentes.
- Solución y explicación presentes.
- Dos distractores por reconocimiento.
- Tres criterios por respuesta abierta.
- Ausencia de opciones duplicadas en una pregunta.

Si falla la estructura del banco, se lanza un error.

Estas comprobaciones NO equivalen a pruebas de interfaz ejecutadas.

## Pruebas manuales recomendadas

El código entregado no se ha ejecutado en un navegador desde la
conversación en la que se generó.

Antes de depender de él para estudiar, comprobar:

- [ ] El mapa muestra nueve salas.
- [ ] La matriz muestra 52 objetivos.
- [ ] La auditoría muestra 7 objetivos parciales.
- [ ] Responder bien incrementa XP.
- [ ] Responder mal resta una vida y muestra explicación.
- [ ] No puede puntuarse varias veces el mismo intento.
- [ ] Una pista impide acreditar la modalidad.
- [ ] Las respuestas abiertas muestran su rúbrica.
- [ ] El jefe se desbloquea tras practicar todos los terminales.
- [ ] Tres respuestas completas vencen al jefe.
- [ ] Llegar a cero vidas permite volver al refugio.
- [ ] Recargar conserva progreso si localStorage está disponible.
- [ ] Exportar e importar conserva el progreso.
- [ ] Importar un JSON inválido muestra un aviso.
- [ ] El juego resulta usable en móvil.
- [ ] Puede recorrerse con teclado.
- [ ] Reducir movimiento desactiva las animaciones.

## Cómo ampliar los apartados pendientes

El banco está dentro de `index.html`, en llamadas a `add(...)`.

Para completar una laguna:

1. Obtener la práctica o fuente autorizada.
2. Añadir una explicación sustentada en ese material.
3. Mejorar el ejercicio práctico y la rúbrica.
4. Actualizar la referencia.
5. Eliminar `gap` únicamente cuando el objetivo esté desarrollado.
6. Revisar de nuevo la matriz de cobertura.

No eliminar las advertencias solamente para que el contador llegue
al 100 %.

## Uso recomendado antes del examen

1. Hacer reconocimiento sin consultar el cuaderno.
2. Explicar la misma idea con palabras propias.
3. Revisar los fallos.
4. Realizar las prácticas reales de comandos y configuración.
5. Resolver los apartados con material pendiente.
6. Terminar con el simulacro mixto.

Ganar al jefe es el incentivo.
Poder explicar por qué funciona la red es el objetivo.
