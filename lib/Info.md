Cómo estructurar mi proyecto?

Arquitectura limpia (Clean Architecture) en Flutter, adaptada con un enfoque feature-first. Este enfoque organiza el código por características o funcionalidades, manteniendo una separación clara de responsabilidades, lo que facilita la escalabilidad y el mantenimiento del proyecto.

lib/config
lib/data/ Implementa la capa de acceso a datos, incluyendo:
models/: Definiciones de modelos de datos.


provider/: Clases que proporcionan datos a la aplicación, posiblemente utilizando patrones como Provider o servicios de red.


repositories/: Implementaciones concretas de los repositorios que interactúan con las fuentes de datos.


lib/presentation/Gestiona la interfaz de usuario y la interacción con el usuario, organizada por características:
pages/: Contiene las diferentes pantallas de la aplicación, organizadas por funcionalidades.


routes/: Define las rutas de navegación entre las diferentes pantallas.


widgets/: Componentes reutilizables en la interfaz de usuario.
