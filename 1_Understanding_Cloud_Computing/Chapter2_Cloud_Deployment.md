## Capítulo 2: Cloud Deployment

### 1. Modelos de despliegue en la nube (Cloud deployment models)
- **Instructora:** Lis Sulmont ([DataCamp](https://app.datacamp.com/learn)).
- **Criterio de elección:** Depende del nivel de control necesario sobre el entorno en la nube, según los requisitos del negocio y el presupuesto. Los tres modelos más comunes son **público**, **privado** e **híbrido**.
- **Nube privada (*Private cloud*):**
  - Uso exclusivo para sus *tenants* mediante enlace o acceso de red configurado por TI; puede gestionarse internamente o por terceros (ej. IBM, RackSpace).
  - Brinda alto control y flexibilidad sobre recursos, almacenamiento, sistema operativo y hardware, pero suele requerir mayor inversión de tiempo y *CapEx* (menor si se delega el hardware).
  - Aplica principios de nube (como virtualización y recursos bajo demanda) y puede ubicarse fuera de las instalaciones.
- **Nube pública (*Public cloud*):**
  - Infraestructura compartida y abierta al público general, propiedad de proveedores como AWS o Azure y accesible por Internet.
  - Permite iniciar rápido con baja inversión inicial y escalar al instante, pero no da acceso físico ni ubicación exacta de los centros de datos por motivos de seguridad.
- **Nube híbrida (*Hybrid cloud*):**
  - Combina dos o más modelos de despliegue conectados por red para compartir datos y servicios (ej. datos sensibles de pacientes en nube privada y *business intelligence* en nube pública).
  - Permite **cloud bursting**: trasladar tráfico adicional a una instancia de nube pública cuando la nube privada llega a su capacidad (como en picos estacionales tipo Black Friday o Boxing Day), optimizando costos con pago por uso.
- **Otros modelos:**
  - **Multicloud:** Combina servicios de distintos proveedores (ej. Azure para respaldos, AWS para alojamiento web y Google Cloud para analítica), aportando flexibilidad y menor dependencia de un solo proveedor; no debe confundirse con el modelo híbrido (que combina modelos de despliegue).
  - **Nube comunitaria (*Community cloud*):** Infraestructura compartida por un grupo o comunidad con intereses, normativas de seguridad, jurisdicción o misión común (ej. instituciones de investigación o agencias gubernamentales), gestionada interna o externamente.

### 2. ¿Privado o público? (Private or public?)
- **Clasificación correcta:**
  - **Private Model:**
    - *Provides an organization with exclusive use of infrastructure*
    - *Can get direct access to all the data centers*
  - **Public Model:**
    - *Usually has the least upfront time investment*
    - *In cloud bursting, overflow traffic is sent to this model*
- **Nota del ejercicio:** No existe un modelo universalmente superior; conviene evaluar los requisitos de seguridad y alternativas intermedias como los modelos híbrido, comunitario o multicloud.

### 3. Elegir el mejor modelo (Pick the best model)
- **Pregunta:** *Below are four statements each describing a deployment model and a use-case. Select the statement that does not describe an appropriate use-case for the given model.*
- **Respuesta seleccionada:** **Hybrid model: Different government agencies need access to tax data.** *(El acceso compartido de múltiples agencias con normativas o misiones comunes encaja mejor en un **Community model**, mientras que el modelo híbrido conecta distintos entornos de despliegue).*

### 4. Regulaciones en la nube (Regulations on the cloud)
- **Instructora:** Lis Sulmont ([DataCamp](https://app.datacamp.com/learn)).
- **Latencia y centros de datos globales:** Tener servidores en distintas regiones (ej. EE. UU., Europa, Sudamérica, África, Asia) reduce la **latencia** (el retraso entre la transmisión y recepción de datos), enviando solicitudes al servidor más cercano al usuario.
- **Implicaciones regulatorias del movimiento de datos:** Enviar datos fuera del país de origen exige cumplir las regulaciones locales del país de origen, de la ubicación del centro de datos y del país sede de la empresa.
- **GDPR (General Data Protection Regulation de la UE):**
  - Regula la recolección, procesamiento y almacenamiento de datos personales de personas en la Unión Europea.
  - Exige consentimiento explícito previo, notificación oportuna de brechas de datos y medidas como cifrado, anonimización o seudonimización según corresponda.
  - Limita sacar datos personales de la UE salvo que se asegure un nivel equivalente de protección.
  - **Multas:** hasta **20 millones de euros** o el **4 %** de los ingresos anuales globales de la empresa (lo que resulte mayor).
- **Datos personales y PII (*Personally Identifiable Information*):**
  - Definidos por la Comisión Europea como cualquier información sobre una persona viva identificada o identificable (incluyendo combinaciones de datos que permitan identificarla).
  - Ejemplos mencionados: nombre, apellido, dirección, correo electrónico, datos de ubicación, dirección IP, origen racial o étnico, opiniones políticas, orientación sexual y datos de salud.
- **Otras normativas y criterio clave:** Existen normativas de protección de datos en países como Brasil, Estados Unidos, Japón, Tailandia y Canadá; revisar la legislación local es clave al elegir dónde ubicar centros de datos.

### 5. Límites de tiempo para almacenar datos (Time limits on storing data)
- **Contexto (extracto de la [Comisión Europea](https://ec.europa.eu/info/law/law-topic/data-protection/reform/rules-business-and-organisations/principles-gdpr/how-long-can-data-be-kept-and-it-necessary-update-it_en) sobre GDPR):** Los datos deben guardarse el menor tiempo posible según el propósito del procesamiento y las obligaciones legales (leyes laborales, fiscales, antifraude, garantías de productos), fijando plazos para eliminarlos o revisarlos.
- **Pregunta:** *How could this rule affect a company using cloud computing?*
- **Respuesta seleccionada:** **If copies of European user data exist on multiple data centers, including disaster recovery backups, companies need to have a robust protocol for making sure every copy is deleted once the time limit elapses.**

### 6. Datos personales (Personal data)
- **Definición de datos personales (GDPR):** Cualquier información vinculada a una persona física viva identificada o identificable (incluidos conjuntos de datos que, al combinarse, identifiquen a alguien).
- **Clasificación del ejercicio:**
  - **Personal data:** *Genetic data*, *Country*, *IP address*, *bob@datacamp.com*, *Salary*.
  - **Not personal data:** *info@datacamp.com* (correo genérico/organizacional).
- **Nota del ejercicio:** Gran parte de los datos recolectados sobre usuarios corresponde a datos personales, lo que impacta directamente cómo se recogen, almacenan y transfieren en la nube.

### 7. Roles en computación en la nube (Cloud computing roles)
- **Instructora:** Lis Sulmont ([DataCamp](https://app.datacamp.com/learn)).
- **Demanda laboral de habilidades en la nube:** Aunque la nube puede reducir costos operativos y de mantenimiento (incluido personal), la demanda de habilidades en la nube es muy alta (listada como la habilidad más demandada en Indeed en febrero de 2020 y segunda habilidad dura tras *blockchain* en LinkedIn, por encima de IA y *machine learning*). Las certificaciones de los grandes proveedores tienen alto valor en el mercado.
- **Roles conocidos de datos y su beneficio en la nube:**
  - *Data scientists:* Ejecutan análisis computacionalmente exigentes más rápido y a menor costo.
  - *Machine learning scientists:* Entrenan y despliegan modelos (especialmente de *deep learning*) aprovechando alta capacidad de cómputo.
  - *Data engineers:* Construyen *pipelines* para ingerir, transformar y almacenar *big data* de forma segura y eficiente.
  - *Data analysts:* Consultan datos en la nube mediante herramientas de *business intelligence* como [Tableau](https://www.datacamp.com/courses/25475/chapters/82110/continue) o [Power BI](https://www.datacamp.com/courses/25475/chapters/82111/continue), facilitando la colaboración sin pasar archivos manualmente entre equipos.
- **Nuevos roles y evolución en la nube (con solapamiento de funciones):**
  - *Cloud architect:* Traduce requisitos técnicos de negocio en una arquitectura de nube escalable, optimizada en costos y con plan de despliegue.
  - *Cloud engineer:* Construye, mantiene y monitorea servicios en la nube y suele encargarse de migraciones desde entornos *on-premise* (en empresas pequeñas puede unirse al rol de arquitecto).
  - *DevOps engineer:* Une desarrollo de software y operaciones de TI (infraestructura como código y automatización), asegurando confiabilidad, disponibilidad y escalabilidad (por ejemplo, escalado automático ante picos de uso o *redeploy* automático ante fallos).
  - *Security engineer:* Define requisitos técnicos de seguridad según la región, evalúa y prueba la seguridad de los datos y protege a la organización y usuarios a nivel técnico.

### 8. Reporte de habilidades en la nube de Microsoft (Microsoft cloud skills report)
- **Contexto:** Encuesta de 2017 de [Microsoft](https://download.microsoft.com/documents/en-gb/Microsoft_Cloud_Skill_Report.pdf) a 250 líderes técnicos en el Reino Unido (segmentada entre organizaciones medianas de 250–999 empleados y grandes de 1000+ empleados).
- **Pregunta:** *What does this plot indicate about cloud skills?*
- **Respuesta seleccionada:** **More than 80% of respondents believe that the right cloud skills will be important or critical to their organization's digital transformation.**

### 9. Roles en la nube (Cloud roles)
- **Clasificación correcta de responsabilidades:**
  - **Cloud Architect:** *Solutions architect of the cloud* / *Design cloud infrastructure based on business requirements*.
  - **Security Engineer:** *Ensure data privacy of users and the organization is protected* / *Spec out technical security requirements based on regulations and business requirements*.
  - **DevOps Engineer:** *Maintain infrastructure through code* / *Ensure reliability, availability, and scalability through automation*.
- **Cierre del capítulo:** Las habilidades en la nube no se limitan a estos perfiles y aplican también para roles como *data scientist* o *data analyst*.