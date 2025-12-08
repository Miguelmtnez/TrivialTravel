# TRIVIALTRAVEL
## Aplicación de Exploración Urbana Gamificada

**Equipo de Desarrollo:**
- Eric Paredes
- Daniel Alcaraz Baixauli
- Miguel Gutiérrez Rico
- Miguel Martinez Rosario

**Fecha:** Diciembre 2025

---

## 1. LA IDEA DE NEGOCIO

### 1.1 Descripción General del Proyecto

TrivialTravel es una aplicación móvil innovadora que revoluciona la forma en que las personas exploran y descubren ciudades, transformando el turismo tradicional en una experiencia interactiva y gamificada. La plataforma combina elementos de juegos de rol, aprendizaje cultural y redes sociales para crear una aventura única en cada viaje.

### 1.2 Problemática Identificada

Los viajeros actuales se enfrentan a varios desafíos:
- **Falta de orientación personalizada:** Las guías turísticas tradicionales no se adaptan a los intereses individuales
- **Experiencias pasivas:** El turismo convencional se limita a visitar lugares sin interacción significativa
- **Desconocimiento de lugares ocultos:** Muchos lugares interesantes pasan desapercibidos para los turistas
- **Dispersión de información:** La información cultural e histórica está fragmentada en múltiples fuentes
- **Falta de motivación:** Los viajeros carecen de incentivos para explorar más allá de los lugares turísticos típicos

### 1.3 Solución Propuesta

TrivialTravel ofrece una solución integral que combina:

**Gamificación del Turismo:**
- Sistema de misiones y desafíos ubicados en puntos de interés reales
- Recompensas, insignias y puntos de experiencia por completar actividades
- Niveles progresivos que desbloquean contenido exclusivo
- Tablas de clasificación para competir con otros viajeros

**Personalización Inteligente:**
- Generación de misiones adaptadas a los intereses del usuario mediante IA
- Rutas dinámicas según el tiempo disponible
- Contenido cultural contextualizado para cada ubicación

**Experiencia Social:**
- Sistema de amigos y grupos de viaje
- Compartir experiencias y recuerdos en tiempo real
- Competencias amistosas y logros compartidos
- Chat grupal e individual

**Diario Digital:**
- Registro automático de viajes y misiones completadas
- Integración de fotos con análisis de IA
- Organización cronológica de experiencias
- Descripciones enriquecidas automáticamente

### 1.4 Valor Diferencial

**Para los Usuarios:**
- Descubrimiento guiado de lugares únicos y poco conocidos
- Aprendizaje activo sobre historia y cultura local
- Experiencia social enriquecida con otros viajeros
- Gamificación que aumenta la motivación para explorar
- Recuerdos organizados y enriquecidos digitalmente

**Para el Sector Turístico:**
- Promoción de lugares menos conocidos
- Aumento del tiempo de permanencia en destinos
- Dispersión del flujo turístico
- Datos valiosos sobre preferencias de viajeros

### 1.5 Modelo de Negocio Potencial

**Freemium:**
- Versión gratuita con funcionalidades básicas
- Premium con misiones exclusivas, análisis avanzados y sin publicidad

**Colaboraciones:**
- Alianzas con oficinas de turismo locales
- Patrocinios de comercios para misiones especiales
- Promoción de eventos culturales

**Publicidad:**
- Anuncios no intrusivos en versión gratuita
- Promoción de experiencias y servicios locales

### 1.6 Mercado Objetivo

**Usuarios Primarios:**
- Millennials y Generación Z (18-35 años) interesados en viajes
- Turistas urbanos que buscan experiencias auténticas
- Estudiantes en programas de intercambio
- Nómadas digitales

**Usuarios Secundarios:**
- Familias que buscan actividades educativas
- Grupos de amigos en viajes recreativos
- Turistas culturales de cualquier edad

**Alcance Geográfico:**
- Inicial: Principales ciudades turísticas de España
- Expansión: Europa y América Latina
- Global: Integración progresiva de ciudades worldwide

---

## 9. ANÁLISIS DE REQUISITOS

### 9.1 Requisitos Funcionales

#### 9.1.1 Gestión de Usuarios y Autenticación

**RF-01: Registro de Usuarios**
- El sistema debe permitir el registro mediante email y contraseña
- El sistema debe validar la unicidad del email
- El sistema debe enviar un email de verificación
- El usuario debe confirmar su cuenta mediante código

**RF-02: Inicio de Sesión**
- El sistema debe autenticar usuarios con credenciales válidas
- El sistema debe mantener la sesión activa
- El sistema debe permitir cerrar sesión

**RF-03: Recuperación de Contraseña**
- El sistema debe permitir restablecer contraseña olvidada
- El sistema debe enviar código de recuperación por email
- El usuario debe poder crear nueva contraseña

**RF-04: Gestión de Perfil**
- El usuario debe poder editar su perfil (nombre, foto, bio)
- El usuario debe poder ver su nivel y experiencia
- El usuario debe poder visualizar sus estadísticas
- El usuario debe poder seleccionar título personalizado

#### 9.1.2 Sistema de Misiones

**RF-05: Visualización de Misiones**
- El sistema debe mostrar misiones disponibles organizadas por ciudad
- Las misiones deben clasificarse en: pendientes, completadas y expiradas
- El sistema debe mostrar detalles: título, descripción, puntos, dificultad
- Las misiones deben mostrar fechas de inicio y fin cuando aplique

**RF-06: Generación de Misiones**
- El sistema debe generar misiones personalizadas mediante IA
- Las misiones deben adaptarse a los intereses del usuario
- El sistema debe crear misiones para ubicaciones específicas
- Las misiones deben incluir información cultural e histórica

**RF-07: Gestión de Misiones**
- Los administradores deben poder crear misiones manualmente
- El sistema debe permitir misiones de evento con fechas específicas
- Los usuarios deben poder aceptar misiones de evento
- El sistema debe asignar misiones a viajes (journeys)

**RF-08: Completar Misiones**
- El usuario debe poder marcar misiones como completadas
- El sistema debe requerir foto de verificación
- El sistema debe analizar la foto mediante IA para validación
- El sistema debe otorgar puntos y experiencia al completar

**RF-09: Pistas de Misiones**
- El sistema debe proporcionar pistas para misiones difíciles
- Las pistas deben generarse mediante IA
- El sistema debe mostrar pistas en un modal informativo

#### 9.1.3 Sistema de Mapas y Navegación

**RF-10: Visualización de Mapa**
- El sistema debe mostrar un mapa interactivo
- El mapa debe indicar ubicaciones de misiones
- El sistema debe mostrar la ubicación actual del usuario
- El mapa debe permitir navegación y zoom

**RF-11: Vista de Globo 3D**
- El sistema debe ofrecer visualización 3D con Cesium
- La vista debe permitir exploración global
- El sistema debe mostrar puntos de interés en 3D

**RF-12: Integración con Servicios de Mapas**
- El sistema debe integrarse con Google Maps
- El sistema debe proporcionar direcciones a ubicaciones
- El sistema debe calcular rutas optimizadas

#### 9.1.4 Sistema de Gamificación

**RF-13: Sistema de Puntos**
- El sistema debe otorgar puntos por completar misiones
- Los puntos varían según dificultad de la misión
- El usuario debe poder consultar su puntuación total
- El sistema debe mantener histórico de puntos

**RF-14: Sistema de Experiencia y Niveles**
- El sistema debe otorgar experiencia por actividades
- El usuario debe subir de nivel al acumular experiencia
- Cada nivel debe requerir más experiencia que el anterior
- El sistema debe notificar al usuario cuando sube de nivel

**RF-15: Sistema de Insignias**
- El sistema debe otorgar insignias por logros específicos:
  - **Misiones:** Completar 1, 5, 10, 25, 50, 100 misiones
  - **Ciudades:** Visitar 1, 3, 5, 10, 20 ciudades
  - **Nivel:** Alcanzar niveles 5, 10, 15, 20, 25
  - **Sociales:** Obtener 1, 5, 10, 25 amigos
  - **Especiales:** "Fotógrafo Viajero" (5 fotos), "Maratonista de Viajes" (10 misiones/día)

**RF-16: Tabla de Clasificación**
- El sistema debe mostrar ranking de usuarios
- El ranking debe ordenarse por puntos totales
- El sistema debe mostrar top 100 usuarios
- El usuario debe poder ver su posición

#### 9.1.5 Sistema Social

**RF-17: Gestión de Amigos**
- El usuario debe poder buscar otros usuarios
- El usuario debe poder enviar solicitudes de amistad
- El sistema debe notificar solicitudes pendientes
- El usuario debe poder aceptar/rechazar solicitudes
- El usuario debe poder eliminar amigos
- El usuario debe poder ver perfil de amigos

**RF-18: Grupos**
- El usuario debe poder crear grupos
- El usuario debe poder invitar amigos a grupos
- Los miembros deben poder abandonar grupos
- El sistema debe mostrar lista de grupos del usuario

**RF-19: Chat y Mensajería**
- El usuario debe poder enviar mensajes privados
- El sistema debe soportar chat grupal
- Los mensajes deben mostrarse en tiempo real
- El sistema debe mantener histórico de conversaciones

**RF-20: Compartir Contenido**
- El usuario debe poder compartir viajes con amigos
- Los amigos deben poder ver viajes compartidos
- El usuario debe poder compartir misiones específicas
- El sistema debe gestionar permisos de visualización

#### 9.1.6 Diario de Viaje

**RF-21: Creación de Entradas**
- El sistema debe crear entradas automáticas al completar misiones
- Las entradas deben incluir: fecha, ubicación, fotos, descripción
- El usuario debe poder agregar notas personales
- El sistema debe generar descripciones mediante IA

**RF-22: Gestión de Diario**
- El usuario debe poder ver todas sus entradas
- Las entradas deben ordenarse cronológicamente
- El usuario debe poder filtrar por fecha o ubicación
- El sistema debe permitir editar entradas

**RF-23: Análisis de Imágenes con IA**
- El sistema debe analizar fotos subidas mediante Google Gemini
- El análisis debe validar la ubicación de la foto
- El sistema debe enriquecer descripciones con información de IA
- El análisis debe proporcionar contexto cultural

#### 9.1.7 Sistema de Viajes (Journeys)

**RF-24: Creación de Viajes**
- El usuario debe poder crear nuevos viajes
- Cada viaje debe asociarse a una ciudad específica
- El sistema debe permitir descripción del viaje
- El viaje debe almacenar fecha de creación

**RF-25: Gestión de Viajes**
- El usuario debe poder ver todos sus viajes
- El sistema debe mostrar misiones asociadas a cada viaje
- El usuario debe poder eliminar viajes
- El sistema debe organizar viajes por ciudad

#### 9.1.8 Panel de Administración

**RF-26: Gestión de Misiones (Admin)**
- Los administradores deben poder crear misiones
- Los administradores deben poder editar misiones existentes
- Los administradores deben poder eliminar misiones
- Los administradores deben poder crear misiones de evento

**RF-27: Gestión de Contenido (Admin)**
- Los administradores deben poder moderar contenido
- Los administradores deben poder gestionar ciudades
- Los administradores deben poder configurar insignias

#### 9.1.9 Notificaciones

**RF-28: Sistema de Notificaciones Push**
- El sistema debe enviar notificaciones para:
  - Nuevas solicitudes de amistad
  - Mensajes recibidos
  - Nuevas misiones disponibles
  - Logros desbloqueados
  - Eventos próximos a expirar
- El usuario debe poder gestionar preferencias de notificaciones

#### 9.1.10 Integración con Servicios Externos

**RF-29: Cloudinary**
- El sistema debe subir imágenes a Cloudinary
- El sistema debe optimizar imágenes automáticamente
- El sistema debe gestionar almacenamiento de fotos

**RF-30: Google Gemini AI**
- El sistema debe usar Gemini para:
  - Generar descripciones de misiones
  - Analizar imágenes de verificación
  - Crear contenido personalizado
  - Proporcionar pistas inteligentes

**RF-31: Clima**
- El sistema debe mostrar pronóstico del clima
- La información debe actualizarse en tiempo real
- El sistema debe mostrar clima para ubicación actual y ciudades

### 9.2 Requisitos No Funcionales

#### 9.2.1 Rendimiento

**RNF-01: Tiempo de Respuesta**
- Las operaciones de lectura no deben superar 2 segundos
- La carga inicial de la aplicación no debe superar 3 segundos
- Las búsquedas deben responder en menos de 1 segundo

**RNF-02: Capacidad**
- El sistema debe soportar al menos 10,000 usuarios concurrentes
- La base de datos debe manejar millones de registros eficientemente

**RNF-03: Escalabilidad**
- La arquitectura debe permitir escalado horizontal
- El sistema debe soportar crecimiento de usuarios sin degradación

#### 9.2.2 Seguridad

**RNF-04: Autenticación y Autorización**
- El sistema debe usar tokens JWT para autenticación
- Las contraseñas deben almacenarse con hash seguro
- El sistema debe implementar políticas de seguridad RLS (Row Level Security)

**RNF-05: Protección de Datos**
- Los datos sensibles deben transmitirse cifrados (HTTPS)
- El sistema debe cumplir con GDPR
- Las APIs deben estar protegidas contra ataques comunes (SQL injection, XSS)

**RNF-06: Privacidad**
- El usuario debe controlar visibilidad de su perfil
- El sistema debe respetar configuraciones de privacidad
- Los datos de ubicación deben manejarse de forma segura

#### 9.2.3 Usabilidad

**RNF-07: Interfaz de Usuario**
- La interfaz debe ser intuitiva y fácil de navegar
- El diseño debe seguir principios de UX/UI modernos
- La aplicación debe ser responsive para diferentes tamaños de pantalla

**RNF-08: Accesibilidad**
- La aplicación debe cumplir estándares de accesibilidad
- El sistema debe soportar diferentes idiomas (i18n)
- La interfaz debe ser usable con lectores de pantalla

**RNF-09: Experiencia Offline**
- La aplicación debe funcionar parcialmente sin conexión
- Los datos deben sincronizarse al recuperar conexión
- El sistema debe notificar al usuario sobre estado de conexión

#### 9.2.4 Disponibilidad

**RNF-10: Uptime**
- El sistema debe tener disponibilidad del 99.5% o superior
- El mantenimiento programado debe notificarse con anticipación

**RNF-11: Recuperación ante Fallos**
- El sistema debe tener backups automáticos diarios
- El tiempo de recuperación ante fallos no debe superar 4 horas

#### 9.2.5 Compatibilidad

**RNF-12: Plataformas**
- La aplicación debe funcionar en iOS y Android
- El sistema debe soportar versiones recientes de sistemas operativos

**RNF-13: Navegadores (Web)**
- La versión web debe funcionar en Chrome, Firefox, Safari, Edge

#### 9.2.6 Mantenibilidad

**RNF-14: Código**
- El código debe seguir estándares de TypeScript/JavaScript
- El proyecto debe tener estructura modular y escalable
- El código debe estar documentado adecuadamente

**RNF-15: Testing**
- El sistema debe incluir tests unitarios
- Las funcionalidades críticas deben tener tests de integración
- El coverage de código debe ser superior al 70%

#### 9.2.7 Portabilidad

**RNF-16: Base de Datos**
- El sistema debe poder migrar entre proveedores cloud
- Los datos deben ser exportables en formatos estándar

### 9.3 Restricciones Técnicas

**Restricción 01: Stack Tecnológico Obligatorio**
- **Frontend Mobile:** React Native con Expo
- **Lenguaje:** TypeScript
- **Estado:** Redux Toolkit
- **Backend:** Node.js con Express
- **Base de Datos:** Supabase (PostgreSQL)
- **Autenticación:** Supabase Auth
- **Almacenamiento:** Cloudinary
- **IA:** Google Gemini API
- **Mapas:** Google Maps API, Cesium

**Restricción 02: APIs de Terceros**
- Dependencia de disponibilidad de Google Gemini API
- Limitaciones de cuota en APIs de terceros
- Costos asociados a llamadas API

**Restricción 03: Dispositivos Móviles**
- Limitaciones de almacenamiento local
- Consumo de batería por uso de GPS
- Variabilidad en capacidades de cámara

### 9.4 Requisitos de Datos

#### 9.4.1 Entidades Principales

**Usuarios (users)**
- id, email, nombre, foto, nivel, experiencia, puntos, bio

**Ciudades (cities)**
- id, nombre, país, coordenadas, descripción

**Misiones/Desafíos (challenges)**
- id, título, descripción, dificultad, puntos, ubicación, ciudad_id, is_event, fecha_inicio, fecha_fin

**Viajes (journeys)**
- id, usuario_id, ciudad_id, descripción, fecha_creación

**Misiones de Viaje (journeys_missions)**
- id, journey_id, challenge_id, completada, fecha_completada, foto_url

**Insignias (badges)**
- id, nombre, descripción, categoría, threshold, icono

**Insignias de Usuario (user_badges)**
- id, usuario_id, badge_id, fecha_desbloqueo

**Amistades (friendships)**
- id, usuario1_id, usuario2_id, estado, fecha_solicitud

**Grupos (groups)**
- id, nombre, descripción, creador_id, fecha_creación

**Mensajes (messages)**
- id, remitente_id, destinatario_id, contenido, fecha, leído

**Diario (journal_entries)**
- id, usuario_id, journey_mission_id, título, contenido, fotos, fecha

#### 9.4.2 Integridad y Consistencia

- Todas las relaciones deben mantener integridad referencial
- Las eliminaciones en cascada deben estar definidas
- Los índices deben optimizar consultas frecuentes
- Las transacciones críticas deben ser ACID

### 9.5 Requisitos de Interfaces

#### 9.5.1 Interfaces de Usuario

**Pantallas de Autenticación:**
- Login
- Registro
- Verificación de email
- Recuperación de contraseña

**Pantallas Principales:**
- Home/Dashboard
- Misiones
- Mapa
- Perfil
- Diario
- Amigos
- Grupos
- Chat
- Leaderboard
- Insignias

**Pantallas Administrativas:**
- Panel de administración
- Creación/edición de misiones
- Gestión de contenido

#### 9.5.2 APIs Externas

- **Supabase REST API:** CRUD de datos
- **Supabase Realtime:** Actualizaciones en tiempo real
- **Google Maps API:** Servicios de mapeo
- **Google Gemini API:** Procesamiento de IA
- **Cloudinary API:** Gestión de imágenes
- **Weather API:** Información meteorológica

### 9.6 Casos de Uso Principales

#### CU-01: Explorar Ciudad
**Actor:** Usuario registrado
**Descripción:** El usuario selecciona una ciudad y recibe misiones personalizadas
**Flujo Principal:**
1. Usuario selecciona ciudad en el mapa
2. Sistema genera misiones personalizadas mediante IA
3. Usuario visualiza misiones disponibles
4. Usuario acepta misión de su interés
5. Sistema agrega misión al viaje del usuario

#### CU-02: Completar Misión
**Actor:** Usuario registrado
**Descripción:** El usuario completa una misión y obtiene recompensas
**Flujo Principal:**
1. Usuario navega a ubicación de la misión
2. Usuario toma foto en el lugar
3. Sistema analiza foto con IA para validación
4. Sistema verifica ubicación mediante GPS
5. Sistema marca misión como completada
6. Sistema otorga puntos y experiencia
7. Sistema crea entrada en el diario
8. Sistema verifica y otorga insignias si aplica
9. Sistema notifica al usuario logros obtenidos

#### CU-03: Conectar con Amigos
**Actor:** Usuario registrado
**Descripción:** El usuario busca y agrega amigos
**Flujo Principal:**
1. Usuario busca otro usuario por nombre/email
2. Usuario envía solicitud de amistad
3. Sistema notifica al destinatario
4. Destinatario acepta solicitud
5. Sistema establece relación de amistad
6. Usuarios pueden ver perfiles y compartir contenido

#### CU-04: Crear y Compartir Viaje
**Actor:** Usuario registrado
**Descripción:** El usuario crea un viaje y lo comparte con amigos
**Flujo Principal:**
1. Usuario crea nuevo viaje seleccionando ciudad
2. Usuario agrega descripción y detalles
3. Usuario completa misiones durante el viaje
4. Usuario comparte viaje con amigos
5. Amigos reciben notificación
6. Amigos pueden visualizar progreso del viaje

### 9.7 Requisitos de Implementación

**Fase 1: MVP (Minimum Viable Product)**
- Autenticación básica
- Sistema de misiones
- Mapa con ubicaciones
- Sistema de puntos básico
- Perfil de usuario

**Fase 2: Gamificación**
- Sistema completo de insignias
- Niveles y experiencia
- Leaderboard
- Sistema de logros

**Fase 3: Social**
- Sistema de amigos
- Chat y mensajería
- Grupos
- Compartir contenido

**Fase 4: IA y Personalización**
- Generación de misiones con IA
- Análisis de imágenes
- Recomendaciones personalizadas
- Contenido dinámico

**Fase 5: Expansión**
- Múltiples idiomas
- Más ciudades
- Panel administrativo completo
- Optimizaciones de rendimiento

### 9.8 Métricas de Éxito

**Métricas de Uso:**
- Número de usuarios activos mensuales (MAU)
- Número de misiones completadas por usuario
- Tiempo promedio en la aplicación
- Tasa de retención (día 1, día 7, día 30)

**Métricas de Engagement:**
- Número de ciudades exploradas por usuario
- Cantidad de fotos subidas
- Interacciones sociales (amigos, mensajes, grupos)
- Insignias desbloqueadas promedio

**Métricas Técnicas:**
- Tiempo de carga de la aplicación
- Tasa de errores
- Disponibilidad del sistema
- Uso de recursos (CPU, memoria, red)

---

## Conclusión

TrivialTravel representa una innovación en el sector del turismo urbano, combinando tecnologías modernas de desarrollo móvil, inteligencia artificial y gamificación para crear una experiencia única de exploración. El proyecto no solo busca satisfacer las necesidades de los viajeros modernos, sino también aportar valor al sector turístico mediante la promoción de lugares menos conocidos y la generación de datos valiosos sobre comportamiento de usuarios.

La arquitectura cliente-servidor propuesta garantiza escalabilidad, seguridad y rendimiento, mientras que el uso de tecnologías modernas como React Native, Supabase y servicios de IA asegura una experiencia de usuario de alta calidad y facilita el mantenimiento y evolución futura del proyecto.
