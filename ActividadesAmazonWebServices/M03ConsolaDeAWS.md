<p align="left">
  <img src="https://semanadelcannabis.cayetano.edu.pe/assets/img/logo-upch.png" width="150">
  <h1 align="center">Módulo 3: Consola de AWS</h1>
</p>

## Terminología
| Término  | Concepto  |
| :------------: | :------------: |
|  Amazon Simple Storage Service (Amazon S3) |  <p align="justify">Servicio que almacena datos para los usuarios en la nube.</p> |
|  Amazon Elastic Compute Cloud (Amazon EC2) |  <p align="justify">Servicio web que ofrece capacidad de cómputo escalable en la nube. Considérelo como alquilar un equipo en la nube.</p> |
| Amazon Elastic Block Store (Amazon EBS)  | <p align="justify">Almacenamiento para instancias EC2 específicas. Considérelo como la unidad de almacenamiento de su instancia EC2.</p>  |
| Amazon Relational Database Service (Amazon RDS)  |  <p align="justify">Es un servicio en la nube que permite a los desarrolladores crear y gestionar bases de datos relacionales de manera eficiente. Imagina una base de datos relacional como una colección de datos donde cada elemento tiene relaciones con otros elementos de la base de datos. Por ejemplo, en una base de datos de transacciones de un almacén, cada cliente estaría relacionado con sus compras específicas.</p> |
|  Amazon DynamoDB | <p align="justify">Servicio de bases de datos no relacionales de AWS. Los datos se almacenan en pares de clave-valor.</p>  |
| AWS Lambda  |  <p align="justify">Lambda le permite ejecutar código sin necesidad de aprovisionar o administrar servidores. Solo pagará por el tiempo de cómputo que consuma. No se cobra nada cuando el código no se está ejecutando.</p> |
|  Amazon Virtual Private Cloud (Amazon VPC) |  <p align="justify">Un servicio que proporciona una red virtual dedicada a su cuenta de AWS. Esta infraestructura está aislada de forma lógica de otras redes virtuales de la nube de AWS. Todos sus servicios de AWS se pueden lanzar desde una VPC. Sirve para proteger los datos y adinistrar quién puede acceder a la red.</p> |
|  AWS Identy and Management (IAM) | <p align="justify">Implica el control de los usuarios que necesiten acceder a recursos informáticos.</p>  |
|  AWS CloudTrail |  <p align="justify">Monitorea todas las acciones que se realizan en su cuenta de AWS por motivos de seguridad.</p> |
|  Amazon CloudWatch |  <p align="justify">CloudWatch es un servicio de supervisión para monitorizar los recursos de AWS y las aplicaciones que ejecuta en AWS.</p> |
|  Amazon Redshift | <p align="justify">El servicio de almacenamiento de datos de AWS puede almacenar enormes cantidades de datos de forma que se puedan consultar rápidamente con fines de inteligencia empresarial.</p>  |

## Antecedentes y conceptos
<p align="justify">
Amazon VPC es la red virtual que define dónde lanza los recursos de AWS. Esta red virtual se parece mucho a una red tradicional que opera en su propio centro de datos, con las ventajas de utilizar la infraestructura escalable de AWS.</p>
<p align= "center">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/c39cf795-7395-414f-912e-321d6bd94884" width="400">
</p>
<p align="justify">
Amazon S3 y Amazon EBS son formas de almacenamiento de datos. Existen algunas diferencias clave:</p>
<p align="justify">
- Amazon EBS solo se puede utilizar cuando se conecta a una instancia EC2 y se puede acceder a Amazon S3 por sí solo.<br>
- Amazon EBS no puede contener tantos datos como Amazon S3.<br>
- Amazon S3 experimenta más retrasos que Amazon EBS al escribir datos.</p>
<div align="center"; style="display: flex; justify-content: space-between;">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/322f25d1-024b-4c9f-a9fa-a63368c328b6" width="390px"/>
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/c78de8cc-7349-40a4-893e-ef10abbd1900" width="450px"/>
</div>
<p align="justify">
Amazon RDS, Amazon Redshift y DynamoDB están relacionados con las bases de datos, pero existen diferencias:</p>
<p align="justify">
- Amazon RDS es la base de datos relacional clásica que utiliza SQL Server, Oracle Database, Amazon Aurora u otros sistemas de bases de datos similares. Considérelo como un libro de calificaciones en el que cada alumno es una fila y todos tienen el mismo número de tareas (columnas) a las que se adjuntan. Las empresas pueden utilizar el código para buscar datos específicos en función de la información de las filas y columnas. Amazon RDS resulta útil para las empresas que almacenan una cantidad moderada de datos de estructura uniforme, lo que significa que cada ID único, como el nombre del estudiante, se adjunta al mismo número de puntos de datos (calificaciones).</p>
<p align= "center">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/45898109-44ff-4e86-91f5-cfe234f43bb8" width="400">
</p>
<p align="justify">
- Amazon Redshift es una base de datos relacional como Amazon RDS, pero está diseñada específicamente para grandes cantidades de datos. Es una herramienta de almacenamiento de datos que es buena para los usuarios que trabajan con big data.</p>
<p align= "center">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/9ccbcbcd-ca4f-4651-ab80-367e63b42625" width="400">
</p>
<p align="justify">
- DynamoDB es una base de datos no relacional, lo que significa que no se pueden utilizar sistemas tradicionales como SQL Server o Aurora. Cada elemento de la base de datos se almacena como un par de clave-valor o como una notación de objetos JavaScript (JSON). Esto significa que cada fila podría tener un número diferente de columnas. No es necesario que todas las entradas se emparejen de la misma manera. Esto permite una flexibilidad en el procesamiento que funciona bien para blogs, juegos y publicidad.</p>
<p align= "center">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/6337d282-5815-4903-80d0-a3318f29487e" width="400">
</p>
<p align="justify">
CloudTrail y CloudWatch son servicios de monitorización en la nube, pero realizan diferentes funciones:</p>
<p align="justify">
- CloudTrail monitorea todas las acciones que los usuarios han realizado en una cuenta de AWS determinada. Esto significa que cada vez que alguien carga datos, ejecuta código, crea una instancia EC2, cambia un tipo de unidad S3 o cualquier otra acción que se pueda realizar en AWS, CloudTrail lo registrará. Esto resulta muy útil por razones de seguridad para que los administradores puedan saber quién está utilizando su cuenta y qué están haciendo. Si algo sale mal o si surge un problema de seguridad, CloudTrail será la mejor prueba para averiguar lo ocurrido.</p>
<p align= "center">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/5e2fef92-ae3a-48e0-8d55-c0361a279462" width="400">
</p>
<p align="justify">
- CloudWatch monitorea lo que hacen los distintos servicios y qué recursos están utilizando. Si CloudTrail monitorea personas, CloudWatch monitorea servicio. CloudWatch es excelente para asegurarse de que sus servicios en la nube funcionan sin problemas y no utilizan más o menos recursos de los esperados, lo que es importante para el seguimiento del presupuesto. CloudWatch es excelente para asegurarse de que todos los recursos están funcionando, lo que puede resultar complicado si una gran empresa utiliza cientos de máquinas y unidades diferentes. Los monitores y alarmas se pueden configurar a través de CloudWatch para iniciar automáticamente una alerta cuando una métrica alcanza un límite específico.</p>
<p align= "center">
  <img src="https://github.com/EdwinJaraOFC/CDRPersonal/assets/150296803/949032e4-16aa-42a3-9624-987f63ddf474" width="400">
</p>

## Actividad 1: Aprender los servicios principales de AWS
#### Describa uno de los usos reales de un servicio de AWS de los que ha aprendido. ¿Cómo ayuda el servicio a la empresa o a la industria que lo utiliza?
<p align="justify">
Un ejemplo del uso real de un servicio de AWS es el empleo de Amazon S3 (Simple Storage Service) por parte de una empresa de medios de comunicación para almacenar y distribuir contenido multimedia. Amazon S3 ofrece almacenamiento escalable y duradero, permitiendo a la empresa almacenar grandes volúmenes de archivos multimedia de manera segura y accesible desde cualquier lugar del mundo. Esto beneficia a la empresa al mejorar la entrega de contenido multimedia a los usuarios, optimizando así la experiencia del cliente y reduciendo los costos de almacenamiento.</p>

#### ¿Qué servicio cree que es el más importante? ¿Qué servicio cree que utilizará probablemente en su área de carrera planificada?
<p align="justify">
En mi opinión, uno de los servicios más importantes de AWS es Amazon EC2 (Elastic Compute Cloud). EC2 proporciona capacidad informática escalable en la nube, lo que permite a las empresas ejecutar aplicaciones y cargas de trabajo de manera eficiente sin la necesidad de invertir en infraestructura física costosa. Para el campo de la ingeniería informática, servicios como AWS Lambda son fundamentales. AWS Lambda permite ejecutar código sin necesidad de gestionar servidores, lo que es esencial para aplicaciones y servicios que requieren alta escalabilidad y flexibilidad, optimizando así el desarrollo y la implementación de sistemas informáticos complejos.</p>

## Actividad 2: Preguntas de enfoque
#### ¿Qué es un servicio en la nube que usa habitualmente? ¿Qué beneficio le proporciona? ¿Tiene algún inconveniente utilizar este servicio en la nube?
<p align="justify">
Un servicio en la nube que uso habitualmente es Google Drive. Me permite almacenar, sincronizar y compartir archivos en línea, lo cual es muy conveniente para acceder a mis documentos desde cualquier dispositivo con conexión a internet. Sin embargo, uno de los posibles inconvenientes es la dependencia de la conexión a internet para acceder a los archivos.</p>

#### La mayoría de ustedes ha utilizado un tipo de servicio en la nube SaaS. En el futuro, ¿cómo podría utilizar un servicio en la nube PaaS o IaaS? ¿Cómo pueden ayudarle los servicios en una carrera profesional o a alcanzar un objetivo?
<p align="justify">
En el futuro, un servicio en la nube IaaS podría ser útil para desplegar servidores virtuales bajo demanda, lo que me permitiría escalar mi infraestructura según sea necesario sin incurrir en costos de hardware fijos. Estos servicios en la nube pueden ayudarme en mi carrera profesional al proporcionarme habilidades relevantes en la tecnología de la nube, lo que es muy demandado en el mercado laboral actual.</p>

#### ¿Qué experiencia, si la hay, tiene con la consola y los servicios de AWS? ¿Cuáles ha usado, qué ha creado, hay alguno del que quiera saber más? 
No he tenido ninguna experiencia usando la consola ni los servicios AWS por el momento.