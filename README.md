# ElNrbrrYELRastafali
Proyectito de Nrbrr Y el Fali



<Planteamiento> 


WEB app -> ???


idea base:
Concepto Simple De un Grid de  A x A para jugar al 3 en raya. en cada casilla habra una frase con un reto que cumplir. 
En el momento en el que se haga un reto se podra poner una ficha y una vez 3 fichas estén seguidas se finalizara el juego mostrando un ganador



<Necesidades Basicas>


Base de Datos para poder almacenar las ideas de la comunidad. 

Seccion (User_Ideas) para poder explorar las ideas de la comunidad o escribir la tuya

Establecer Conexion J Vs J para poder interactuar y que cada uno ponga sus fichas. 


<Formato de Ficheros> (Gracias CharYIPIYI)



my-project/                         # → Repositorio raíz (Git)
├── README.md                       # Guía rápida de instalación y uso
├── .gitignore                      # Ignora node_modules, target/, .env, etc.
├── docker/                         # Configuración de contenedores opcional
│   ├── backend.Dockerfile
│   └── frontend.Dockerfile
├── scripts/                        # Scripts auxiliares (bash, powershell, etc.)
│   └── init-db.sql
├── docs/                           # Documentación, diagramas, ADRs…
│   └── architecture.png
├── frontend/                       # ——— Angular ——————————————————————
│   ├── angular.json
│   ├── package.json
│   ├── tsconfig.json
│   └── src/
│       ├── main.ts                 # Bootstrap Angular
│       ├── index.html              # Raíz de la SPA
│       ├── styles.scss             # Estilos globales
│       ├── environments/           # env.ts y env.prod.ts
│       └── app/
│           ├── core/               # Servicios singleton (Auth, HTTP interceptors)
│           ├── shared/             # Componentes, pipes y directivas reutilizables
│           ├── features/           # Módulos de funcionalidad (lazy‑loaded)
│           │   └── users/
│           │       ├── pages/
│           │       ├── components/
│           │       ├── users-routing.module.ts
│           │       └── users.module.ts
│           ├── assets/             # Imágenes, fuentes, i18n…
│           ├── app-routing.module.ts
│           └── app.module.ts
├── backend/                        # ——— Spring Boot ————————————————————
│   ├── pom.xml                     # Dependencias y plugins Maven
│   └── src/
│       ├── main/
│       │   ├── java/com/example/   # Paquete base
│       │   │   ├── DemoApplication.java
│       │   │   ├── config/         # Configuración (CORS, seguridad, mapeo modelo)
│       │   │   ├── controller/     # REST controllers ↔️ /api/**
│       │   │   ├── service/        # Lógica de negocio
│       │   │   ├── repository/     # Interfaces JPA / consultas
│       │   │   └── model/          # Entidades y DTOs
│       │   └── resources/
│       │       ├── application.yml # Propiedades (perfiles dev, prod, test)
│       │       ├── db/             # Migraciones Flyway/Liquibase
│       │       └── static/         # Archivos servidos (swagger-ui, etc.)
│       └── test/
│           └── java/com/example/   # Pruebas unitarias y de integración
└── infra/                          # IaC (Terraform, Ansible, GitHub Actions, etc.)
    └── staging.tf



<Planteaminetos a estudiar> 


Planteamiento Inicial -> Empezar con el juego en si en un motor grafico (Unity) realizar el intercambio de informacion a traves de una pagina web gestionada por nosotros y definir outputs a unity (No se si se puede hacer)

Planteamiento Inicial 2 -> Crear El juego directamente en  el navegador, Gestionar el intercambio de informacion en web con Spring, Rest y angular. 

Planteamiento Inicial 3 -> Crear Directamente el juego en Unity Crear una base de datos integrada en Unity (No se si se puede)



<Como gestionar la BDD> 


Actores Involucrados -> USUARIOS -> Tiene Informarcion Privada del Usuario.
                        Mensajes -> Mensajes que se van a poder poner en el juego.
                        Centro de Mensajeria -> Contiene los mensajes que ponen los Usuarios y los relaciona para poder gestionarlos. 
                        Mensajes Asociados -> Mensajes que se Guarda Un usuario para poder incluirlos en el tablero. 
                        Centro de Amigos -> Establece las relaciones de los amigos mediante ID. -> Necesitaria incluir busqueda por nombre si el juego escala. 
                        Centro de 
                        





<Sugerencias a estudiar> 


Capacidad de Poner fichas sin necesidad de turnos para cumplir retos -> es necesario una figura de Juez 

Poner boosts (Para mas adelante) que hagan que la experiencia mejore -> Poner una ficha a un rival si este hace un reto de x manera. Poder modificar un reto que este haciendo el rival etc...


