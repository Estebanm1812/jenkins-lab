# Jenkins Lab

## Ejecutar Docker Compose

Para ejecutar Docker Compose, asegúrate de que tengas Docker Compose instalado en tu sistema. Luego, sigue estos pasos:

1. Navega a la ubicación donde se encuentra tu archivo `docker-compose.yml`.

2. Ejecuta el siguiente comando en tu terminal para iniciar los contenedores definidos en el archivo `docker-compose.yml`:

```bash
docker-compose up -d
```

3. Extraer passwords

```bash
docker logs id_container
```

```bash
docker exec id_container cat /var/jenkins_home/secrets/initialAdminPassword
```
4. Se Inicia sesion Con la contraseña obtenida en el paso anterior

5. Posteriormente se instala el Plugin de node.js
<img width="1420" alt="Captura de pantalla 2024-04-24 a la(s) 2 08 03 p  m" src="https://github.com/Estebanm1812/jenkins-lab/assets/69942961/029eaa38-2eb7-444f-9d4d-d10af47a18f7">

6. Despues se realiza el tool de Node.js
<img width="1192" alt="Captura de pantalla 2024-04-24 a la(s) 2 06 31 p  m" src="https://github.com/Estebanm1812/jenkins-lab/assets/69942961/b8dd088a-24df-4f30-b418-86779b601009">
7. Seguido a esto se crea un nuevo proyecto libre
<img width="878" alt="Captura de pantalla 2024-04-24 a la(s) 2 09 24 p  m" src="https://github.com/Estebanm1812/jenkins-lab/assets/69942961/67c48ddd-9d98-4d1d-9ec6-3059502b8713">
8. Se configura la conexion con el repositorio de Git
<img width="981" alt="Captura de pantalla 2024-04-24 a la(s) 2 11 50 p  m" src="https://github.com/Estebanm1812/jenkins-lab/assets/69942961/017a9348-197a-4bca-8fa5-82c893a810a8">
9.  Se cambia la rama donde se aplicara la automatizacion
<img width="981" alt="Captura de pantalla 2024-04-24 a la(s) 2 12 44 p  m" src="https://github.com/Estebanm1812/jenkins-lab/assets/69942961/a2459462-b7be-449a-bb99-603c62ca5007">
10. Se Modifica el entorno de ejecucion para inlcuir el Node.js
<img width="981" alt="Captura de pantalla 2024-04-24 a la(s) 2 14 27 p  m" src="https://github.com/Estebanm1812/jenkins-lab/assets/69942961/cfd7f53a-16f4-4695-9a7b-f4a73c093eb7">
11. Se Añade un Build Step en Script de Shell
<img width="282" alt="Captura de pantalla 2024-04-24 a la(s) 2 15 07 p  m" src="https://github.com/Estebanm1812/jenkins-lab/assets/69942961/84b1d93b-eb73-496c-81a8-772dbc8dbfe7">
Con los siguientes comandos
<img width="975" alt="Captura de pantalla 2024-04-24 a la(s) 2 17 18 p  m" src="https://github.com/Estebanm1812/jenkins-lab/assets/69942961/9834b354-40c3-49a5-b1d0-671ca6f8492d">
12. Guardar los cambios
