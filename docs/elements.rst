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

.. toctree::
   :maxdepth: 1

   cerif_xml_publication_entity
   cerif_xml_product_entity
   cerif_xml_patent_entity

   cerif_xml_person_entity
   cerif_xml_organisation_entity

   cerif_xml_project_entity
   cerif_xml_funding_entity
   
   cerif_xml_service_entity
   cerif_xml_equipment_entity
   
   cerif_xml_event_entity
