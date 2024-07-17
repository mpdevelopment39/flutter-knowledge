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
   - <strong>The Cocktail:</strong> Empresa en la que me encuentro actualmente trabajando 100% en proyectos Flutter como Senior Developer.
   - <strong>Opendit:</strong> Mi último proyecto profesional y el más amplio hasta la fecha. Este fue el primer proyecto en el que trabaje en un equipo de Producto, muy diferente a la manera de funcionar en un equipo de desarrollo de software. En este caso no era un proyecto cerrado sino un proyecto que continuamente estaba en iteración, añadiendoles nuevas funcionalidades, realizando cambios en las interfaces y mejorando el rendimiento. Este proyecto incluía las siguientes funcionalidades entre  otras:
      -  Autenticación vía usuario y contraseña y Magic-Link
      -  Implementación de deep-linking para reseteo de contraseña y verificación de registro.
      -  Implementación de sistema de desvío de llamadas con Audio y video de entrada y audio de salida a través de WebRTC y Callkit entre otros.
      -  Implementación de cambios en la app en tiempo real vía websockets.
      -  Implementación de un registro de actividad con visualización de todos los eventos realizados por los usuarios.
      -  Implementación de un sistema para realizar apertura de puertas físicas a través de diferentes medios:
          - Vía in-app a través de un slider.
          - Vía forcetouch.
          - Vía widgets en iOS y Android.
      - Implementación de sistema de analítica completo con las herramientas de Segment,Amplitude,Smartlook.
      - Implementación de herramientas de marketing para la comunicación con los usuarios a través de OneSignal.
      - Testing completo de la app (Unitarios, de Widgets y de integración).
      - Implementación de base de datos local con cache a través de Isar para mejorar la carga inicial de los datos.
      - Implementación de sistema de suscripciones a través de Qonversion, permitiendo a los usuarios tener una suscripción mensual o anual y acceder a un plan premium con funcionalides ilimitadas.
   - <strong>Softphone Alisys:</strong> Tras finalizar el proyecto anterior, la empresa quedó muy satisfecha con el trabajo realizado y decidieron acometer un proyecto interno y que lo llevasemos a cabo con la misma tecnología, por lo que me propusieron comenzar este proyecto. En el tiempo que estuve en la compañía, me dió tiempo a dejar preparada la arquitectura inicial del proyecto y a implementar todo el diseño de interfaces de la aplicación completa así como el sistema de diseño.
   - <strong>Asamblea de Madrid:</strong> Este fue el primer proyecto profesional en el que participé con está tecnología. Fue un proyecto muy motivador e inspirador, ya que era el principal desarrollador del proyecto, junto con otra persona a la que tuve que formar en dicha tecnología para que me ayudase a llegar en plazos a la hora de realizar la entrega. Consistía en una aplicación para iOS (Concretamente iPhones 8 y 11) para los diputados de la Asamblea de Madrid. En epoca COVID, para evitar congestiones y que los diputados tuviesen que ir presencialmente a la Asamblea decidieron desarrollar un proyecto, en este caso una app móvil que incluía las siguientes funcionalidades entre otras:
       - Autenticación vía usuario y contraseña
       - Autenticación vía biometría (FaceId y TouchId)
       - Posibilidad de escuchar el audio de los plenos en tiempo real a traves de WebRTC.
       - Posibilidad de realizar las votaciones vía telemáticas a través de websockets.
       - Visualización del orden de los plenos, votaciones pendientes, votaciones ya realizadas...
