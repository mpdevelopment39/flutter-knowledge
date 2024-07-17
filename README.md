# Flutter Knowledge
Repo para documentar y explicar mis conocimientos y experiencia en Flutter

## Arquitectura

Me parece indispensable seguir unas buenas practicas a la hora de desarrollar y sin duda una de las mejores es respetar y cumplir con una buena arquitectura.
Suelo estructurar y organizar todos los proyectos en los que trabajo de la misma forma para trabajar de la manera más óptima y productiva, ya que me permite mantener y evolucionar los proyectos mucho mejor al largo plazo así como hacerlos escalables y más entendibles. Es fundamental respetar la abstracción de las diferentes capas para evitar el acoplamiento y poder hacer cualquier actualización a futuro de una manera sencilla, además de conseguir tener un código testeable y que cumpla con los principios SOLID. 

Las capas en las que estructuro mis proyectos son las siguientes:

- <strong>UI/Presentation.</strong> Donde defino todo lo que tenga que ver con la interfaz de la aplicación, páginas, componentes/widgets, gestión de estados con riverpod(Notifiers,states)...
- <strong>Domain.</strong> Donde defino nuestras entidades de dominio que utilizaremos a lo largo de la aplicación así como los repositorios y casos de uso.
- <strong>Data.</strong> Donde defino la implementación de nuestros repositorios (Obtención de datos de backend/apis, bbdd, preferencias locales...) y las entidades o modelos de data como las respuestas de dichas fuentes de datos.
- <strong>App/Config.</strong> Donde defino archivos de configuración globales de toda la aplicación como constantes, gestión de rutas, inyección de dependencias, helpers...
 
NOTA: En la capa data suelo optar por utilizar únicamente los repositorios, sin necesidad de crear una capa adicional como son los datasources, para mantener los proyectos lo más sencillo posible. Si se diera el caso de que para determinada funcionalidad tuvieramos dos fuentes de datos, por ejemplo, un backend y una bbdd local con información cacheada podríamos tener esta capa y definir en cada momento que datasource o fuente de datos queremos implementar en nuestros repositorios.

## Proyectos

 ### Personales
   - He desarrollado decenas de aplicaciones por mi cuenta con esta tecnología para publicar en las stores y monetizarlas a través de anuncios.
     Mi actividad como autónomo consistía en lo siguiente:
      1. Analizar el mercado para encontrar nichos de aplicaciones que tuviesen demanda y poca competencia. Revisando los volumenes de búsquedas, los valores asociados a ingresos publiciarios(Ecpms,cpcs...)
      2. Realizar un diseño inicial vía herramientas de diseño como Adobe XD o Figma para no empezar a desarrollar sobre un folio en blanco.
      3. Desarrollar la aplicación correspondiente, añadiendole las funcionalidades base y la monetización a través de anuncios.
      4. Crear los recursos gráficos para publicar en la store. Iconos, screenshots...
      5. Realizar ASO (App Store Optimization) analizando las keywords para conseguir posicionar la aplicación lo más alto posible en las stores y consecuentemente conseguir más descargas orgánicas.
      6. Iterar la aplicación si veo que tiene cogida y descargas en el mercado para añadir nuevas funcionalidades si los usuarios lo requieren.
    
   - Empecé desarrollando aplicaciones sencillas y cuyo desarrollo me llevase poco tiempo para conseguir publicar la mayor cantidad posible de aplicaciones y obtener unos ingresos recurrentes que me permitisen mantenerme económicamente. Posteriormente, comencé a desarrollar proyectos más complejos y que me motivaban más, pero que también requerían mucho más trabajo y dedicación. Todavía sigo trabajando en varios proyectos de este modo con varios compañeros que me acompañan en esta aventura, desde amigos Backends, hasta amigos especializados en Marketing y posicionamiento.

 ### Profesionales
   - 
