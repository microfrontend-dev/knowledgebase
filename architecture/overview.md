# Overview

## Complexity

**System complexity**  
The complexity and difficulty of understanding the whole system and the integration between the single system.

**Module complexity**  
The complexity of a single module. Thats what a developer has to work with on a daily basis.

**Rule of thumb**  
The more modules the higher the system complexity but the lower the individual module complexity.

## Architecture Comparison

| Architecture | Build & Deploy | Integration | Backend | Simple Build | Bundle Size & App Performance | UX | Developer Scalability | Technical Lock in & Migration | Shared Responsibility & Autonomy |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Monolith | One | No Integration |  | ++ | ++ | ++ | -- | -- | -- |
| Modular Monolith | One | Build Time |  | + | ++ | ++ | + | -- | + |
| Self-Contained System | Separate | Run Time |  | - | - | - | ++ | + | ++ |
| Microfrontend | Separate | Run Time |  | --  | -- | - | ++ | ++ | ++ |

