# Taller Docker (COMCOM)

### Motivación:
Manejar paquetes de forma centralizada / abstraerse del SO 

### Contenedores: Es un tipo de virtualización?
No, no es una virtualizacion completa, se apoya fuertemente en el kernel de Linux

### Imagenes de Containers
Es un archivo que incluye todos los archivos, binarios, bibliotecas y configuraciones para levantar el contenedor en un container engine.

### Registry de contenedores
Es un servicio en donde podemos almacenar imagenes de contenedores, compartirlas con otros usuarios y versionarlas/administrarlas de forma centralizada. <br> El mas popular y estandar es **Docker Hub**

### 1 App = 1 Contenedor
Si bien (probablemente) no rompa nada, es ideal mantener una imagen por cada contenedor (1 FROM )

### DockerFile
El dockerFile es el documento que compila la imagen, usando una sintaxis especifica de Docker y es sincrónico. El orden de las instrucciones es importante y existen **layers** que permite modificar la imagen sin recompilar los comandos ejecutados antes del nuevo agregado

### Docker compose
Arma un archivo de configuración para que Docker lo setee. <br> Facilita levantar, detener y escalar aplicaciones completas con un solo comando: docker-compose up y docker-compose down. Además, podemos incluir mas de un container adentro del archivo para levantar todo lo que necesitemos para la ejecución

### Networks 
Redes virtuales para contectar contenedores entre si y con el host.