1. Introducción
---------------
Estas directrices describen el perfil CERIF-XML para que los sistemas de gestión de información científica (CRIS) implementados en el Perú sean compatibles con la plataforma digital de la Red Nacional de Información en Ciencia, Tecnología e Innovación - Proyecto #PerúCRIS. La presente guía está basada y es completamente compatible con el documento OpenAIRE Guidelines for CRIS Managers 1.1 . Incluye definiciones para cada uno de las entidades y elementos de información, así como la referencia a las taxonomías y vocabularios controlados a ser empleados. Además la guía diferencia campos obligatorios y recomendados para diversos tipos de instituciones, tales como universidades, institutos de investigación y entidades financiadoras.

1.1 Objetivo
~~~~~~~~~~~~
Las directrices proporcionan orientación para que los administradores de CRIS expongan sus metadatos de forma compatible con la plataforma del Proyecto #PerúCRIS. Al implementar las directrices, los administradores de CRIS apoyan la inclusión y, por tanto, la reutilización de los metadatos de sus sistemas dentro de la plataforma del Proyecto #PerúCRIS. Para los desarrolladores de plataformas CRIS, las directrices proporcionan orientación para añadir funcionalidades de apoyo a los gestores y usuarios de CRIS. El intercambio de información entre los distintos sistemas CRIS y la infraestructura del Proyecto #PerúCRIS es un ejemplo de intercambio de datos punto a punto entre sistemas CRIS, ya que la propia plataforma del Proyecto #PerúCRIS es un sistema CRIS.

1.2 CERIF-CRIS
~~~~~~~~~~~~~~
El Common European Research Information Format (CERIF) es un modelo de datos estándar de información sobre investigación y una recomendación de la Unión Europea a sus Estados miembros. La Unión Europea transfirió el cuidado y la custodia del CERIF a euroCRIS < http://www.eurocris.org>, una organización, sin fines de lucro, dedicada a la interoperabilidad de los CRIS. Además de un modelo de dominio y un modelo de datos formal, CERIF incluye un mecanismo para construir perfiles XML (subconjuntos especializados) para escenarios específicos de intercambio de información. El perfil CERIF del Proyecto #PerúCRIS admite la recolección e importación de metadatos desde otros sistemas CRIS.

1.3 Sugerencias y comentarios
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
La presente guía se elabora y se perfecciona constantemente en colaboración con instituciones públicas y privadas que realizan y financian actividades de ciencia, tecnología e innovación .

Todos los comentarios y sugerencias para estas directrices, deben dirigirse a: 
sdgic-perucris@concytec.gob.pe 

2. Elementos de información CRIS relevantes para el Proyecto #PerúCRIS
----------------------------------------------------------------------
El CERIF es un modelo integral para el ámbito de la investigación científica. Sólo un segmento de esa información es relevante para el Proyecto #PerúCRIS. Por ejemplo, las publicaciones, los productos (incluidos los conjuntos de datos de investigación y los programas informáticos) y los eventos entran en el ámbito del perfil del Proyecto #PerúCRIS, mientras que los datos sobre premiaciones o direcciones domiciliarias no necesariamente. El siguiente diagrama muestra el segmento del modelo CERIF que se está utilizando en esta versión de la Guía #PerúCRIS:

“cerif_secciones“ 

Figura 1 â€“ Entidades CERIF XML usadas adoptadas por el Proyecto #PerúCRIS 
Fuente: OPENAIRE, 2019.


El modelo CERIF permite clasificar los objetos de información de investigación según su tipo, estado, tema, etc. y expresar los tipos de relaciones entre ellos. Sin embargo, no establece los vocabularios semánticos que se utilizarán para tales clasificaciones; CERIF sólo recomienda aquellos que pueden tener una aplicabilidad común. Para que la comunicación de información tenga éxito, cualquier perfil CERIF necesita especificar los vocabularios semánticos para que los productores sepan qué generar y los consumidores sepan que pueden obtener.

El perfil CERIF del Proyecto #PerúCRIS hace precisamente esto y recomienda los vocabularios que se deben utilizar. Un ejemplo de ello es que los diferentes tipos de resultados de investigación se expresan utilizando el vocabulario COAR (COAR Resource Types). El CERIF tiene tres entidades que representan los resultados de la investigación: publicaciones, productos y patentes. El vocabulario COAR se dividió en sub-vocabularios separados para ser usados con las respectivas entidades.

Las entidades que aborda esta guía son las siguientes:

* Publication
* Product
* Patent
* Person
* OrgUnit
* Project
* Funding
* Service
* Equipment
* Event

A continuación se definen las entidades, elementos y sub-elementos de datos CERIF para el intercambio de datos entre los sistemas CRIS individuales y la plataforma del Proyecto #PerúCRIS. El importante resaltar que el uso de los elementos de datos y los vocabularios definidos es obligatorio, es decir, no se pueden utilizar otros elementos de datos o vocabularios para los datos CERIF XML expuestos por los sistemas CRIS a la plataforma del Proyecto #PerúCRIS. Los vocabularios proceden de fuentes externas relevantes; y en algunos casos se basan en la semántica CERIF 1.5. Finalmente es importante destacar que es posible crear extensiones en la fase de revisión de estas directrices.
