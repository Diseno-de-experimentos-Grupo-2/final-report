# Capítulo V: Product Implementation

## 5.1. Software Configuration Management

### 5.1.1. Software Development Environment Configuration
En esta sección se detallan los productos de software utilizados para el desarrollo del proyecto, organizados por etapa:

**Producto UX/UI Design**
- [Figma](https://www.figma.com/) – Diseño colaborativo de interfaces, wireframes y prototipos.
- [Lucidchart](https://lucid.app/) – Diagramas de flujo, arquitectura de software y base de datos.
- [Uxpressia](https://uxpressia.com/) – Creación de *customer journey maps* y mapas de empatía.
- [Structurizr](https://structurizr.com/) – Modelado de arquitectura orientada a dominios.

**Software Development**
- [IntelliJ IDEA](https://www.jetbrains.com/idea/) – IDE principal para backend Java/Kotlin.
- [Visual Studio Code](https://code.visualstudio.com/) – Editor liviano para frontend web y scripts.
- [GitHub](https://github.com/) – Control de versiones y repositorios colaborativos.
- [HTML5](https://www.w3.org/TR/html52/), [CSS3](https://www.w3.org/Style/CSS/), JavaScript/TypeScript – Tecnologías base para la aplicación web.
- Frameworks: Angular para frontend, SpringBoot para la API, Android Studio para móvil.

---

### 5.1.2. Source Code Management
El proyecto utiliza **GitHub** como plataforma de control de versiones bajo el modelo **GitFlow**, que permite una colaboración ordenada y controlada.

- **Organización:** https://github.com/Diseno-de-experimentos-Grupo-2 <br><br>
- **Repositorio informe:** https://github.com/Diseno-de-experimentos-Grupo-2/final-report <br><br>
- **Repositorio landing page:** https://github.com/Diseno-de-experimentos-Grupo-2/entrena.pe---landing <br><br>
- **Repositorio frontend web:** https://github.com/Diseno-de-experimentos-Grupo-2/entrena-frontend<br><br>
- **Repositorio backend:** https://github.com/Diseno-de-experimentos-Grupo-2/entrena-platform<br><br>
- **Repositorio app movil:** https://github.com/Diseno-de-experimentos-Grupo-2/appMovil-entrena.pe <br><br>

**Ramas principales**
- `master` – Rama de integración de nuevas funcionalidades.
- Ramas por capítulo: `chapter-1` … `chapter-5`.
- Ramas por feature: `feature/login`, `feature/api-endpoints`, etc.

---

### 5.1.3. Source Code Style Guide & Conventions
**Principios Generales**
- **Idioma:** Inglés para nombres de variables, clases y métodos.
- **Legibilidad:** Nombres claros y descriptivos.

**HTML & CSS**
- Archivos terminan en `.html` y `.css`.
- Clases y archivos en *kebab-case*: `main-header`, `product-card`.
- Uso correcto de etiquetas semánticas (`<header>`, `<section>`, `<footer>`).
- Imágenes con `alt` y atributos `aria-*` para accesibilidad.

**JavaScript / TypeScript**
- Estándar [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript).
- Variables y funciones en *camelCase*, clases en *PascalCase*.
- Comentarios JSDoc para funciones y componentes.

---

### 5.1.4. Software Deployment Configuration
La **landing page** se despliega mediante **GitHub Pages**, mientras que la API y el backend serverless se despliegan en **AWS Lambda**.

- **Landing page repositorio:** https://github.com/Diseno-de-experimentos-Grupo-2/entrena.pe---landing <br><br>
- **Landing page desplegado:** https://diseno-de-experimentos-grupo-2.github.io/entrena.pe---landing/

Evidencias de despliegue:  
<img width="1595" height="848" alt="image" src="https://github.com/user-attachments/assets/e03a7a04-f088-4a37-ade8-7149ef7ea016" />

---

## 5.2. Product Implementation & Deployment
### 5.2.1. Sprint Backlogs
Cada sprint siguió el marco Scrum con reuniones de *planning*, *review* y *retrospective*.

| Sprint | Fecha inicio | Objetivo principal                             |
|--------|--------------|------------------------------------------------|
| 1      | 07-09-2025   | Diseño y despliegue de landing page responsiva |
| 2      | 12-09-2025   | Implementación de API REST y base de datos     |
| 3      | 13-09-2025   | Desarrollo de frontend web con Angular         |

**USER STORIES TERMINADAS**:

| US ID | Título                                 | Descripción                                                                                                                                       |
|-------|----------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------|
| US03  | Crear nuevo ejercicio                  | Como entrenador, quiero crear un nuevo ejercicio para ampliar mi biblioteca personalizada                                                         |
| US08  | Crear rutina personalizada             | Como entrenador quiero crear rutinas de entrenamiento personalizadas para mis clientes para adaptar los ejercicios según sus objetivos            |
| US16  | Ver rutinas organizadas                | Como deportista quiero ver mis rutinas organizadas por fecha y tipo para seguir un plan estructurado                                              |
| US17  | Ver detalles de rutina                 | Como deportista quiero consultar los detalles de cada rutina para ejecutar correctamente los ejercicios                                           |
| US01  | Buscar ejercicios en la biblioteca     | Como entrenador, quiero buscar ejercicios en la biblioteca para encontrarlos rápidamente y asignarlos a una rutina                                |

---

### 5.2.2. Implemented Landing Page Evidence
Se desarrolló una **landing page responsive** para presentar el producto, optimizada para SEO y compatible con dispositivos móviles.  
Evidencia:  
<img width="1599" height="849" alt="image" src="https://github.com/user-attachments/assets/1b367e3f-b339-4fb3-9962-ee9fff88c4b4" />


---

### 5.2.3. Implemented Frontend-Web Application Evidence
Aplicación web construida en **Angular**, con diseño modular y consumo de la API REST.  
Evidencia de pantallas clave:  

<img width="1532" height="701" alt="image" src="https://github.com/user-attachments/assets/e5bdf858-7f7e-4b2b-b268-7e80277df46e" />

<img width="1641" height="592" alt="image" src="https://github.com/user-attachments/assets/4ddabae8-61be-471d-96bf-50e26ea44b10" />

<img width="1641" height="592" alt="image" src="https://github.com/user-attachments/assets/282ff04c-ae2c-487e-8900-54b035c76133" />

<img width="1382" height="729" alt="image" src="https://github.com/user-attachments/assets/9715698d-9723-40b7-b7e3-17911b81391b" />

---

### 5.2.4. Acuerdo de Servicio – SaaS
Se redactó un **Service Level Agreement (SLA)** que define:
- Nivel de disponibilidad: 99.5 %.
- Políticas de soporte y mantenimiento.
- Responsabilidades del proveedor y del cliente.

---

### 5.2.5. Implemented Native-Mobile Application Evidence
Aplicación móvil en **Android Studio**, disponible para Android en fase beta.  
Evidencia de instalación y pantallas:  
<img width="696" height="854" alt="image" src="https://github.com/user-attachments/assets/6cbaac7e-86c6-4a11-9bee-21535f25a167" />
<img width="697" height="850" alt="image" src="https://github.com/user-attachments/assets/c27890ea-9f50-440a-a33f-5cad275d55b8" />
<img width="686" height="844" alt="image" src="https://github.com/user-attachments/assets/9aa1f8ea-a28c-4802-b000-bc64bf553afd" />


---

### 5.2.6. Implemented RESTful API and/or Serverless Backend Evidence
API desarrollada en **SpringBoot**, con base de datos en **MySQL**.  
Evidencia de endpoints en Swagger: 

<img width="1458" height="545" alt="image" src="https://github.com/user-attachments/assets/3aaed504-c190-4fec-a885-b1d8c213bdf4" />
<img width="1450" height="329" alt="image" src="https://github.com/user-attachments/assets/b5a9b545-9d97-45b7-a247-425f353b840f" />

---

### 5.2.7. RESTful API documentation


---

### 5.2.8. Team Collaboration Insights

  

---

## 5.3. Video About-the-Product
Video demostrativo de las principales funcionalidades del producto, incluyendo la landing page, la aplicación web y la aplicación móvil.  


