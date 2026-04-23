# Week-11

## Entrega Release 2

La **Week 11** esta enfocada en la **entrega de Release 2** de FarmaExpres.

Este repositorio empaqueta la presentacion publica del release en una experiencia local en HTML con:

- una narrativa clara que inicia desde la problematica de la farmacia
- un recorrido por roles para **Administrador**, **Farmaceutico** y **Auditor**
- evidencia en video de los flujos principales del producto
- evidencia del manejo de ambientes **dev**, **qa** y **main**
- una explicacion sencilla de **Liquibase** en lenguaje entendible para negocio

El objetivo de esta semana no es agregar una funcionalidad aislada nueva dentro de este repositorio, sino **consolidar, presentar y documentar Release 2** de una manera clara para publico, jurado o stakeholders.

---

## Tabla de contenido

- [Que cambio desde Week 10](#que-cambio-desde-week-10)
- [Balance de continuidad entre Weeks 9, 10 y 11](#balance-de-continuidad-entre-weeks-9-10-y-11)
- [Que incluye este repositorio](#que-incluye-este-repositorio)
- [Estructura de la presentacion](#estructura-de-la-presentacion)
- [Evidencias](#evidencias)
- [Como ejecutarlo en local](#como-ejecutarlo-en-local)
- [Notas de Release 2](#notas-de-release-2)

---

## Que cambio desde Week 10

Durante la **Week 10**, el equipo estuvo concentrado en cerrar y consolidar la implementacion tanto en backend como en frontend:

- cierre de backend desde **HU-011** hasta **HU-016**
- ajustes de backend alrededor de **HU-AC02**
- documentacion QA de frontend desde **HU-QA-FE-08** hasta **HU-QA-FE-12**
- preparacion base de **HU-017**, relacionada con versionado de base de datos

En la **Week 11**, el enfoque cambio desde el cierre de implementacion hacia el **empaquetado y la entrega de Release 2**:

- el release ahora se presenta mediante una experiencia local en HTML
- el recorrido se organiza con flujos reales del producto, no con fragmentos de codigo
- la entrega explica como se comporta la plataforma segun cada rol y escenario operativo
- la evidencia incluye la separacion de ambientes entre **dev**, **qa** y **main**
- la entrega resalta la estrategia de versionado de base de datos con **Liquibase**
- el repositorio incorpora evidencia visual de la trazabilidad hasta **Release.2**

### Resumen de Week 11

- Esta semana es principalmente una **semana de entrega de release y consolidacion de evidencias**.
- El valor tecnico mas visible ligado a Release 2 esta en:
  - separacion de ambientes
  - trazabilidad del release
  - versionado de base de datos con Liquibase
- Si la pregunta es si este repositorio agrega una historia de usuario completamente nueva por si solo, la respuesta es **no**.
- Si la pregunta es si Release 2 aporta valor consolidado frente a Week 10, la respuesta es **si**:
  - mejor preparacion para entregar
  - comunicacion mas clara para el publico
  - evidencias mas fuertes de despliegue y estabilidad de datos

---

## Balance de continuidad entre Weeks 9, 10 y 11

Esta seccion resume la continuidad del trabajo entre las semanas anteriores y la entrega actual de **Week 11**, tomando como base lo que se documento y consolido en **Weeks 9 y 10**.

### Que se hizo?

- En **Week 9** se organizo la base documental y de trazabilidad para backend y frontend.
- En backend se consolidaron las historias **HU-007** a **HU-011** con enfoque en alcance, criterios de aceptacion, endpoints y componentes tecnicos.
- En frontend se validaron y documentaron los flujos QA de **HU-QA-FE-02** y **HU-QA-FE-07**, especialmente autenticacion e historial de movimientos.
- En **Week 10** se avanzo en el cierre tecnico del bloque backend desde **HU-011** hasta **HU-016**, junto con **HU-AC02** y cambios de ramas de apoyo.
- Tambien en Week 10 se documentaron y consolidaron en frontend las historias **HU-QA-FE-08** hasta **HU-QA-FE-12**, ampliando la cobertura funcional y de validacion.
- En **Week 11** no se abrio una historia de usuario aislada nueva, sino que se tomo todo ese avance acumulado y se transformo en una **entrega de Release 2 entendible para publico**.
- Para ello se construyo una presentacion HTML local con narrativa de producto, videos funcionales por rol, evidencia de ambientes **dev**, **qa** y **main**, trazabilidad hacia **Release.2** y explicacion de **Liquibase** como respaldo de estabilidad y confianza.

### Que falto?

- Aunque Week 10 dejo un cierre fuerte de implementacion y QA, todavia quedaban validaciones integrales de extremo a extremo por robustecer entre backend, frontend y despliegue.
- Week 11 se concentro en **empaquetar y comunicar** el valor del producto, por lo que no se destino a abrir un nuevo bloque funcional independiente.
- Sigue siendo importante fortalecer pruebas de regresion completas para asegurar que la consolidacion del release no afecte funcionalidades previas.
- Tambien queda como paso posterior llevar esta evidencia a un nivel mas cercano a despliegue final o validacion de salida completamente estabilizada.

### Que se hara?

- A partir de esta entrega, el siguiente paso natural es usar la base consolidada de Release 2 para atender retroalimentacion de la demostracion y ajustar detalles funcionales o visuales que se detecten.
- Se debera continuar con validaciones integradas backend-frontend para confirmar que lo documentado, probado y presentado se mantenga consistente en escenarios reales.
- Se espera fortalecer aun mas la disciplina de ambientes, la trazabilidad de promotion y el versionado de base de datos para futuras entregas.
- Si surgen nuevas iteraciones, estas ya partiran de una base mucho mas madura: documentada en Week 9, consolidada tecnicamente en Week 10 y presentada como producto en Week 11.

---

## Que incluye este repositorio

### Archivos principales de la presentacion

- `release2-presentation.html`
- `release2-presentation.css`
- `release2-presentation.js`

### Videos de demostracion

- `Videos/1.mp4` hasta `Videos/15.mp4`

Estos videos soportan el recorrido funcional de:

- gestion de productos por el Administrador
- control de usuarios por el Administrador
- reportes, filtros y alertas
- operaciones de inventario del Farmaceutico
- revision y verificacion del Auditor

### Recursos de apoyo

- `assets/evidence-ambientes.svg`
- `assets/evidence-release.svg`
- `assets/evidence-liquibase-structure.svg`
- `assets/evidence-liquibase-flow.svg`
- `assets/screenshots/overview.png`

### Ayuda para correrlo en local

- `presentacion-local.cmd`

Este archivo inicia un servidor local y abre la presentacion en el navegador para evitar problemas con la reproduccion de videos MP4 desde archivo local.

---

## Estructura de la presentacion

La presentacion HTML esta organizada en cuatro momentos principales:

### 1. Problematica

La presentacion comienza explicando el problema operativo real de una farmacia pequena:

- poca claridad sobre el inventario disponible
- riesgo de vencimientos o perdidas por caducidad
- baja trazabilidad de entradas y salidas
- reportes tardios para tomar decisiones

### 2. Funcionamiento del producto

La seccion del producto muestra como FarmaExpres organiza la operacion por rol:

- **Administrador**
  - crear producto
  - modificar producto
  - eliminar producto
  - crear usuario
  - bloquear usuario
  - modificar usuario y cambiar contrasena
  - revisar movimientos
  - ver reportes y Excel
  - consultar alertas
- **Farmaceutico**
  - revisar inventario
  - registrar entrada
  - registrar salida
- **Auditor**
  - revisar inventario
  - inspeccionar movimientos por filtros
  - revisar reportes

### 3. Diversificacion de ambientes

Release 2 demuestra que el producto no solo funciona, sino que tambien esta organizado para crecer:

- `dev` para desarrollo activo
- `qa` para validacion
- `main` para entrega estable

Esta parte conecta la entrega con disciplina operativa real y no solo con una interfaz visual.

### 4. Liquibase explicado en lenguaje claro

Liquibase se presenta como una pieza de confianza del producto:

- los cambios de base de datos quedan versionados
- los ambientes se mantienen alineados
- los servicios validan el esquema antes de operar
- el producto puede crecer sin perder control sobre sus datos

---

## Evidencias

### Vista general de la presentacion HTML

![Vista general de Release 2](assets/screenshots/overview.png)

### Evidencia de ambientes

![Evidencia de ambientes](assets/evidence-ambientes.svg)

### Evidencia de trazabilidad del release

![Evidencia de trazabilidad del release](assets/evidence-release.svg)

### Evidencia de estructura Liquibase

![Evidencia de estructura Liquibase](assets/evidence-liquibase-structure.svg)

### Evidencia de ejecucion Liquibase

![Evidencia de ejecucion Liquibase](assets/evidence-liquibase-flow.svg)

---

## Como ejecutarlo en local

### Opcion 1: clonar y abrir

```bash
git clone https://github.com/Marlon271/Week-11.git
cd Week-11
```

Luego abre:

- `release2-presentation.html`

En muchos equipos esto funciona de inmediato y es la manera mas rapida de revisar la entrega.

### Opcion 2: recomendada para la exposicion

Si el navegador bloquea la reproduccion local de los MP4 o quieres una presentacion mas estable, ejecuta:

- `presentacion-local.cmd`

Esto va a:

- iniciar un servidor HTTP local
- abrir automaticamente la presentacion en el navegador

---

## Notas de Release 2

Este repositorio esta preparado para soportar la **presentacion publica de Release 2**.

Su estructura esta pensada para que la explicacion se mantenga dentro del mismo HTML:

- sin navegar a paginas externas
- con lenguaje claro y entendible
- con prioridad en el valor del producto por encima del codigo
- con evidencia visual sobre operacion, release y estabilidad

Desde la perspectiva del release, la Week 11 demuestra que FarmaExpres no solo muestra pantallas, sino tambien:

- una historia de producto coherente
- manejo disciplinado de ambientes
- trazabilidad de promotion hacia Release.2
- evolucion controlada de la base de datos

Eso es lo que permite presentar Release 2 como producto y no solo como ejercicio tecnico.
