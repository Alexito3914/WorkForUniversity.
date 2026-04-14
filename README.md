# WorkForUniversity.
1. Objetivo
Se ha realizado una primera versión funcional del proyecto en Django a partir del documento maestro de requisitos. En esta práctica no se implementan todavía todos los requisitos funcionales, pero sí una base sólida del dominio, la navegación inicial y la instrumentación para depuración.
2. Modelado del dominio
Se han definido las entidades principales del sistema: Titulación, Año Académico, Curso, Profesor, Estudiante, Aula, Asignatura, Oferta de Asignatura, Franja Horaria, Disponibilidad del Profesor, Horario, Entrada de Horario, Matrícula y Perfil de Usuario. Las relaciones principales son: una Titulación tiene varios Cursos; un Curso pertenece a una Titulación y a un Año Académico; una Asignatura puede ofertarse en varios Cursos; cada Oferta de Asignatura se asocia a un único Profesor y una única Aula; un Horario contiene múltiples Entradas de Horario; y cada Estudiante puede matricularse en varias Ofertas de Asignatura.
3. Implementación realizada
Se ha creado la estructura del proyecto Django con una app principal llamada “horarios”. Se han implementado los modelos y su registro en el panel de administración. También se han definido dos vistas: la home de la aplicación (/) y una segunda URL de ejemplo (/dashboard/), cada una con su template HTML correspondiente.
4. django-debug-toolbar
Se ha añadido el paquete django-debug-toolbar en el proyecto, incluyendo su configuración en INSTALLED_APPS, MIDDLEWARE y urlpatterns. Con ello se podrán visualizar peticiones HTTP, tiempos de respuesta y consultas SQL durante las pruebas locales, tal y como pide la práctica.
5. Resultado
La V1 permite arrancar el servidor local, acceder a la home, navegar a otra ruta con su template y dejar preparado el proyecto para continuar en prácticas posteriores con lógica de generación de horarios, validaciones y control de roles más completo.
