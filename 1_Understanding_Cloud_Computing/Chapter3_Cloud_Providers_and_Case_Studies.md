## Capítulo 3: The Cloud Infrastructure Market

- **Instructor:** Iason Prassides

### 1. An overview of providers
- Alcance del capítulo: presenta los principales proveedores de nube según participación de mercado, servicios clave, fortalezas, clientes y casos de estudio, además de sus principales servicios de almacenamiento, cómputo y bases de datos.
- Mercado dinámico: el panorama cloud cambia continuamente (los productos pueden quedar obsoletos, cambiar de nombre o ser reemplazados, y los clientes pueden cambiar de proveedor).
- Participación de mercado y líderes: al cierre de 2023, las cuotas de mercado (basadas en PaaS, IaaS y nube privada alojada) muestran tres actores principales en los que se enfocará el capítulo.
- Valor de la computación en la nube: implementar correctamente servicios IaaS, PaaS y soluciones cloud en general ayuda a las empresas a ganar agilidad, eficiencia e innovación, reducir costos y centrarse en su negocio principal.
- Selección de proveedor y evaluación previa: elegir proveedor depende de las necesidades de la empresa (apoyándose en especialistas internos y contactando directamente a los proveedores) y exige evaluar:
  - Costos actuales de infraestructura, operación de centros de datos y gestión de hardware físico y almacenamiento.
  - Costo de retirar, migrar o reconstruir aplicaciones para la nube.
  - Costo de incorporar especialistas en nube al equipo.
  - Beneficios para la empresa y sus clientes, junto con los riesgos potenciales de migrar.

### 2. The Big Three
- Pregunta: Which three cloud services make up the big three?
- Clasificación en pantalla:
  - Big three: Microsoft Azure, Amazon Web Services, Google Cloud.
  - Other cloud providers: IBM Cloud, Oracle Cloud, Alibaba Cloud.

### 3. The risk of vendor lock-in
- Definición: el vendor lock-in ocurre cuando un cliente que usa un servicio en la nube no puede cambiar fácilmente al producto o servicio de un competidor.
- Pregunta: What are things a company can do to avoid vendor lock-in?
- Respuesta seleccionada: All of the above are good strategies for avoiding vendor lock-in (implementar estrategias multicloud o híbridas, invertir en estándares y tecnologías abiertas, y evitar contratos a largo plazo negociando flexibilidad contractual).

### 4. Amazon Web Services
- Historia y liderazgo en el mercado: Amazon Web Services (AWS) se lanzó en 2006 (dos años antes que Google Cloud y cuatro antes que Microsoft Azure). Su ventaja como first mover le permitió desarrollar más de 175 servicios (cómputo, almacenamiento, analítica, seguridad, aplicaciones empresariales y machine learning). Al cierre de 2023, lideraba el mercado con el 31 % de participación total.
- Servicios clave de infraestructura:
  - S3 (Simple Storage Service): almacenamiento de archivos.
  - EC2 (Elastic Compute Cloud): cómputo.
  - RDS (Relational Database Service): bases de datos relacionales.
- Servicios clave de datos y machine learning:
  - Redshift: data warehouse administrado a escala de petabytes.
  - Kinesis: analítica y datos en tiempo real.
  - SageMaker: plataforma de machine learning para analítica predictiva.
- Clientes destacados: Disney, Verizon y Deloitte, entre otros.
- Caso de estudio - NerdWallet: utilizaba cómputo y contenedores de Amazon y sumó SageMaker para construir, entrenar y desplegar modelos en un solo lugar integrado con sus instancias de cómputo:
  - El lanzamiento de modelos pasó de meses a días, liberando tiempo para estrategia y otros proyectos.
  - Los costos de entrenamiento bajaron un 75 % al usar instancias bajo demanda (on-demand) en lugar de mantener una activa continuamente.

### 5. AWS or not AWS!
- Pregunta: Which of the following is Not a cloud service offered by AWS?
- Respuesta seleccionada: BigQuery (BigQuery corresponde a Google Cloud, mientras que Simple Storage Service [S3], Kinesis y Redshift forman parte de AWS).

### 6. NerdWallet
- Pregunta: What was the outcome of NerdWallet's move to Amazon SageMaker?
- Respuesta seleccionada: Models now take days to train instead of months. (Al centralizar el desarrollo, entrenamiento y despliegue de modelos en Amazon SageMaker y usar instancias bajo demanda, NerdWallet redujo drásticamente el tiempo de lanzamiento de modelos y abarató sus costos de entrenamiento).

### 7. Microsoft Azure
- Posicionamiento y participación de mercado: Microsoft comenzó adaptando a la nube productos como Microsoft Office, Windows Server y SQL Server, con estrecha integración y fuerte fidelidad de clientes. Al cierre de 2023, ocupaba el segundo lugar detrás de AWS con 24 % de participación total de mercado.
- Servicios clave de infraestructura y bases de datos:
  - Azure Blob Storage: almacenamiento de archivos.
  - Azure Virtual Machines: cómputo.
  - Azure SQL Database: bases de datos.
- Microsoft Fabric y servicios de datos:
  - Microsoft Fabric: solución SaaS empresarial que unifica movimiento de datos, ciencia de datos, analítica en tiempo real y business intelligence.
  - Azure Data Lake Storage: almacenamiento previo a tareas de preparación de datos.
  - Azure Stream Analytics: analítica en tiempo real.
  - Azure Machine Learning: entrenamiento y despliegue de modelos de machine learning.
- Clientes destacados: Siemens, The World Bank y L'Oréal, entre otros.
- Caso de estudio - The Ottawa Hospital: hospital canadiense que atiende a 1,2 millones de personas y gestiona millones de registros médicos:
  - Buscaba mejorar el intercambio de historias clínicas electrónicas entre sedes y redes asociadas, manteniendo el almacenamiento principal on-premise (más económico allí) y trasladando el sitio de recuperación ante desastres (disaster recovery, para continuidad tras sismos, incendios o ciberataques) a la nube por su alto costo local.
  - Implementó un entorno IaaS en Azure con Azure Storage (imágenes médicas) y Azure Site Recovery (activación automática ante pérdida de datos), sincronizado continuamente con sus bases on-premise.
  - Resultados: respaldo de 700 terabytes, soporte para 5.300 usuarios concurrentes, cumplimiento de la normativa canadiense de privacidad en salud (Personal Health Information Protection Act), implementación en menos de tres meses y ahorro cercano al 50 % en costos de recuperación ante desastres.

### 8. Which service to pick?
- Clasificación del ejercicio:
  - Data Science and Analytics Services: Azure Stream Analytics, Azure Machine Learning.
  - Data Storage Services: Azure Data Lake, Azure SQL Database.
- Nota del ejercicio: Azure ofrece más de 200 productos y servicios; distinguir entre almacenamiento y analítica/ciencia de datos ayuda a elegir la herramienta adecuada según el flujo de trabajo.

### 9. The Ottawa Hospital
- Pregunta: Why did the Ottawa hospital decide to use Microsoft Azure Site Recovery?
- Respuesta seleccionada: They needed a reliable solution to protect their data and essential operations during a disaster. (Azure Site Recovery permite activar automáticamente el respaldo en la nube ante incidentes o fallos críticos para mantener la continuidad operativa y proteger los datos del hospital).

### 10. Google Cloud
- Enfoque y participación de mercado: Google Cloud apuesta por el multicloud y por evitar el vendor lock-in. En 2019 lanzó Google Cloud Anthos para gestionar y desplegar cargas de trabajo de forma unificada entre entornos on-premise y distintos proveedores sin depender de distintos entornos o APIs. Al cierre de 2023, contaba con 11 % de cuota de mercado, detrás de AWS y Microsoft Azure.
- Servicios clave de infraestructura:
  - Google Cloud Storage: almacenamiento de archivos.
  - Google Cloud Compute Engine: cómputo.
  - Google Cloud SQL: bases de datos.
- Servicios clave de datos y machine learning:
  - BigQuery: data warehousing para consultar y analizar datos a escala.
  - Dataflow: servicio administrado de analítica en streaming.
  - AutoML: conjunto de herramientas y servicios de machine learning.
- Clientes destacados: HSBC, PayPal y Vodafone, entre otros.
- Caso de estudio - Lush: fabricante de cosméticos vegetarianos cuya mayor temporada de ventas es Boxing Day, donde sufría caídas web al superar las 12 transacciones por segundo:
  - Migró toda su infraestructura (apps móviles, e-commerce, sistemas de tienda, datos de clientes y productos, y 17 sitios web) a Google Cloud durante diciembre (su mes más ocupado).
  - Usó Google Cloud Compute Engine para probar, modificar y desplegar con rapidez bajo plazos ajustados, y Google Cloud SQL para alojar sus datos.
  - Resultados: cero caídas en Boxing Day, 40 % de reducción en costos de hosting y lanzamiento de una aplicación de reconocimiento de imágenes para identificar productos y consultar ingredientes o instrucciones al reducir el empaque.

### 11. Lush migration
- Pregunta: The international cosmetics company Lush migrated their entire infrastructure to Google Cloud. What was the expected outcome?
- Respuesta seleccionada: Lush wanted to improve the scalability and availability of their e-commerce platform when traffic increases. (Lush buscaba evitar las caídas de su plataforma de comercio electrónico durante picos de tráfico como Boxing Day y mejorar su escalabilidad y disponibilidad en Google Cloud).

### 12. True or false?
- Clasificación correcta de afirmaciones:
  - True:
    - Amazon Web Services offers a breadth of cloud solutions for a lot of different areas. (Más de 175 servicios en cómputo, almacenamiento, bases de datos, analítica, redes, móvil, herramientas de desarrollo/gestión, IoT, seguridad, aplicaciones empresariales, machine learning y robótica).
    - Google Cloud has a service to allow customers to manage and deploy workloads across several cloud providers. (Como Google Cloud Anthos).
    - Microsoft Azure provides integration with other Microsoft products such as the Office Suite or SQL Server.
  - False:
    - Compute Engine, Big Query, Blob Storage and SageMaker are all AWS services. (Mezcla servicios de Google Cloud como Compute Engine y BigQuery, de Azure como Blob Storage y de AWS como SageMaker).
    - Microsoft was the first mover on the cloud infrastructure market. (AWS fue el primero en lanzarse en 2006).

### 13. Cloud providers and their services
- Clasificación correcta de servicios:
  - File storage: Amazon S3, Azure file storage.
  - Computation: Azure Virtual Machines, Amazon EC2.
  - Databases: Google BigQuery, Amazon Redshift.

### 14. Congratulations!
- Cierre del curso: recapitula el recorrido completo por los fundamentos de computación en la nube:
  - Capítulo 1 (Introduction to cloud computing): funcionamiento de la nube, sus ventajas clave y modelos de servicio principales.
  - Capítulo 2 (Cloud strategies): modelos de despliegue, impacto de regulaciones (como GDPR y protección de datos) y roles necesarios para construir y mantener infraestructuras en la nube.
  - Capítulo 3 (The cloud infrastructure market): principales proveedores de infraestructura (AWS, Microsoft Azure y Google Cloud), su posicionamiento, servicios clave, clientes y casos de estudio.
- Próximos pasos recomendados: consultar a especialistas internos de nube, explorar sitios de proveedores o contactarles directamente, y continuar con cursos enfocados en la gestión de aplicaciones en la nube en DataCamp.
