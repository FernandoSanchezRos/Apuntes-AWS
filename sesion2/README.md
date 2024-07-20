# Sesión 2: Manejo de IAM y EC2

## Documentación

- [Anexo-Grupos_vs_Roles.pdf](docs/Anexo-Grupos_vs_Roles.pdf): Documento que compara las diferencias entre grupos y roles de IAM.
- [Clase2.1-IAM.pdf](docs/Clase2.1-IAM.pdf.pdf): Definición, características y usos de AWS IAM.
- [Clase2.2-EC2.pdf](docs/Clase2.2-EC2.pdf): Definición, características y usos de AWS EC2.
- [Practica1-Gestion_Usuarios_IAM.pdf](docs/Practica1-Gestion_Usuarios_IAM.pdf): Guía sobre cómo crear y gestionar usuarios IAM usando boto3.
- [Practica2-Instancias_EC2.pdf](docs/Practica2-Instancias_EC2.pdf): Guía sobre cómo crear y gestionar instancias EC2 usando boto3.

## Notebooks

- [Gestion_Usuarios_IAM.ipynb](notebooks/Gestion_Usuarios_IAM.ipynb): Notebook de Jupyter con ejemplos de creación y gestión de usuarios IAM usando boto3.
- [Instancias_EC2.ipynb](notebooks/Instancias_EC2.ipynb): Notebook de Jupyter con ejemplos de creación y gestión de instancias EC2 usando boto3.

## Configuración de Credenciales de AWS

Para ejecutar el código en los notebooks, necesitarás tener configuradas tus credenciales de AWS en tu sistema. Aquí tienes cómo hacerlo:

1. **Instalar AWS CLI**:

   Si no tienes AWS CLI instalado, puedes seguir las instrucciones [aquí](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html).

2. **Configurar tus credenciales**:

   Ejecuta el siguiente comando y sigue las instrucciones para introducir tu `AWS Access Key ID` y `AWS Secret Access Key`:

   ```bash
   aws configure
   ```

   Esto creará un archivo de configuración en `~/.aws/credentials` con tus credenciales de AWS.

3. **Verificar configuración**:

   Puedes verificar que tus credenciales están configuradas correctamente ejecutando:

   ```bash
   aws sts get-caller-identity
   ```

   Deberías ver una respuesta que incluya tu `Account` y `Arn`.

## Uso

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/FernandoSanchezRos/Apuntes-AWS.git
   cd Apuntes-AWS/session1
   ```

2. Revisar la documentación en la carpeta `/docs`.

3. Configurar tus credenciales de AWS siguiendo las instrucciones en la sección anterior.

4. Abrir y ejecutar los notebooks en la carpeta `/notebooks` usando Jupyter Notebook:
   ```bash
   jupyter notebook notebooks/Creacion-Sesion-AWS.ipynb
   ```

## Contribuir

Las contribuciones son bienvenidas. Por favor, abre un issue o envía un pull request para cualquier mejora o corrección.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.
