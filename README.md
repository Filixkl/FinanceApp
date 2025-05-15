# FinanceApp: Aplicación de Finanzas Personales

**FinanceApp** es una aplicación multiplataforma desarrollada con Kotlin Multiplatform, orientada a ayudar a los usuarios a **gestionar sus inversiones personales** de forma centralizada, sin necesidad de conectarse directamente a bancos ni plataformas de intercambio. Esta app sirve como un "cuaderno inteligente" para llevar el control de activos de diversos tipos, calcular rentabilidades y visualizar datos en tiempo real.

## Objetivo del proyecto

El objetivo de esta aplicación es **unificar la gestión de todos los activos financieros** (acciones, ETFs, criptomonedas, bienes raíces, metales preciosos, activos personales, etc.) en una sola plataforma accesible, privada y flexible. Los usuarios podrán registrar y gestionar inversiones manualmente o importar valores conocidos, sin comprometer su privacidad bancaria.

Este proyecto se realiza como **Trabajo de Fin de Ciclo** del grado superior de Desarrollo de Aplicaciones Multiplataforma (DAM).

---

## Arquitectura y tecnologías

La arquitectura del proyecto sigue un enfoque moderno, modular y multiplataforma:

### Frontend
- **Jetpack Compose Multiplatform** para UI nativa en Android (y escalable a iOS, escritorio, web).
- Diseño claro/oscuro, con enfoque en usabilidad y accesibilidad.
- Visualización de datos financieros mediante gráficos interactivos.

### Persistencia
- **Base de datos local**: SQLite con [SQLDelight] o Realm.
- **Sincronización remota**: backend desarrollado con Ktor y PostgreSQL.

### Autenticación
- Inicio de sesión con **Google Sign-In** mediante Firebase Authentication.

### Backend
- API REST con **Ktor**
- Base de datos **PostgreSQL**
- Desplegado con **Docker** (opcionalmente en Kubernetes)

### DevOps y testing
- CI/CD con **GitHub Actions**
- Pruebas unitarias y de integración con herramientas nativas de Kotlin
- Backend dockerizado, opción a desplegar en clúster local con **Minikube/Kubernetes**

---

## Funcionalidades

- [x] Registro e inicio de sesión con cuenta de Google
- [x] Añadir, editar y eliminar inversiones personalizadas
- [x] Clasificación por tipos de activo
- [x] Cálculo de rentabilidad (esperada y obtenida)
- [x] Visualización de la cartera total y distribución en gráficos
- [x] Sincronización entre base de datos local y nube
- [x] Modo oscuro y claro
- [x] Actualización de precios manual o vía API (si se implementa)

---

## 📅 Roadmap del proyecto (4 semanas)

### 🗓️ Semana 1 – Fundamentos
- [ ] Definir requisitos funcionales y técnicos
- [ ] Elegir tecnologías definitivas (Realm o SQLDelight, Ktor, Compose)
- [ ] Crear estructura base del proyecto
- [ ] Configurar CI/CD básico en GitHub
- [ ] Empezar UI base (login, dashboard)

### 🗓️ Semana 2 – Autenticación y CRUD
- [ ] Integrar Google Sign-In con Firebase
- [ ] Crear estructura de base de datos local
- [ ] Implementar creación y edición de inversiones
- [ ] Backend en Ktor con conexión PostgreSQL
- [ ] Dockerizar el backend

### 🗓️ Semana 3 – Sincronización y análisis
- [ ] Sincronizar datos entre app y backend
- [ ] Implementar cálculo de rentabilidad
- [ ] Añadir visualización gráfica de cartera
- [ ] Mejorar diseño UI/UX

### 🗓️ Semana 4 – Tests, CI/CD y documentación
- [ ] Pruebas unitarias e integración
- [ ] Terminar CI/CD (despliegue automático)
- [ ] Documentación técnica y memoria del TFG
- [ ] Opcional: Despliegue de backend en Kubernetes (Minikube o GKE)

---

## 🔐 Seguridad y privacidad

- Los datos del usuario se almacenan de forma local y en el servidor personal.
- No hay conexión directa a bancos ni plataformas externas que comprometan datos financieros reales.
- Autenticación segura mediante Google y Firebase.

---

## 📖 Licencia

Este proyecto se realiza con fines educativos como Trabajo de Fin de Ciclo. Puedes usarlo como referencia para otros proyectos de gestión personal.

---

## ✍️ Autor

**Filixkl**  
Desarrollador de Aplicaciones Multiplataforma (DAM)  
