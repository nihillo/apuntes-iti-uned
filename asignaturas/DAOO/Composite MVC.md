## Responsabilidades
### Modelo
- Administrar los datos de la aplicación y proveer los servicios asociados
- Proveer un acceso a los datos y los servicios para las vistas y los controladores
- Registrar, como observadores, las vistas y los controladores que dependan de la actualización del modelo
- Notificar a los observadores en caso de actualización
### Vista
- Mostrar la información al usuario
- Actualizar la representación gráfica en caso de producirse alguna actualización del modelo
- Buscar los datos del modelo
- Ofrecer posibilidades de manipulación de representación gráfica para el controlador asociado a la vista
- Crear e inicializar el controlador asociado
### Controlador
- Administrar los eventos que provienen del usuario
- Traducir los eventos en consultas para el modelo o para la vista (manipulación de la representación gráfica)
- Adaptar, si fuera necesario, los distintos componentes del controlador cuando se produce alguna actualización en el modelo
