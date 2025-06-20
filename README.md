README - INSTRUCCIONES PARA EJECUCIÓN DE LA COLECCIÓN API_OPEN_CART

REQUISITOS:
- Tener instalado Node.js y Newman:
* npm install -g newman

#Instalar dependencias
* npm install

#Ejecutar el script
   al ejecutar el script se ejecutan los test deben ejecutarse en el orden que se encuentran en el archivo postman_collection.json

* npm run test

EJECUCIÓN:
1. Abrir terminal o CMD en la carpeta del proyecto.
2. Ejecutar el siguiente comando:
* newman run Api_OpenCart.postman_collection.json -r cli,html

    - Esto genera un reporte en consola y en formato HTML si deseas.
    - Puedes agregar variables de entorno si deseas parametrizar, por ejemplo:
* newman run Api_OpenCart.postman_collection.json --env-var email=correo@prueba.com

CONTENIDO DEL ZIP:
- Api_OpenCart.postman_collection.json (colección principal)
- informe.txt (hallazgos, resultados, recomendaciones)
- readme.txt (instrucciones para ejecutar la prueba desde cero)
