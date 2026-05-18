# 🎮 Catálogo de Videojuegos Volvo 

Proyecto académico desarrollado para la asignatura de Desarrollo Fullstack.
Sistema backend basado en microservicios para gestionar un catálogo de
videojuegos con géneros, plataformas, estudios, usuarios y reseñas.

## Integrantes
- Emiliano Cerda
- Katalina Diaz

## Tecnologías
Java · Spring Boot · Spring Data JPA · WebClient · MySQL · Lombok · Maven

## Microservicios

| Servicio          | Puerto | Descripción                              |
|-------------------|--------|------------------------------------------|
| Genre Service     | 8081   | Gestión de géneros de videojuegos        |
| Platform Service  | 8082   | Gestión de plataformas disponibles       |
| Game Service      | 8083   | Catálogo principal de juegos             |
| Studio Service    | 8084   | Gestión de estudios desarrolladores      |
| User Service      | 8085   | Registro y consulta de usuarios          |
| Review Service    | 8086   | Reseñas y puntuaciones de la comunidad   |

## Arquitectura
Cada microservicio es independiente con su propia base de datos MySQL.
La comunicación entre servicios se realiza mediante WebClient (WebFlux)
usando el patrón Request/Response DTO.