# Registro de Errores

Completar una fila por cada error detectado.

| N | Archivo | Problema encontrado | Como lo detectaron | Solucion aplicada |
|---|---------|---------------------|--------------------|-------------------|
| 1 | src/ejemplo.js | El token no se verificaba | Prueba manual de ruta protegida | Se uso jwt.verify con manejo de excepcion |
| 2 | src/app.js | Fallaba la lectura del body de postman | Prueba manual de ruta protegida | Agregado del uso de express.json() |
| 3 | src/utils/token.js | la funcion SignToken no devolvia nada | Prueba en postman | reescritura del exports |
| 4 | src/data/db.js | Existia "users" como una constante con un unico usuario | seguimiento de ruta | pasar "users" a una no constante |
| 5 | src/controllers/userController.js | el users.find para el get de usuarios estaba mal escrito | revision manual de codigo | reescritura de codigo|

## Guia de calidad para el informe

No alcanza con escribir "habia un error y lo arreglamos".

En cada caso expliquen:

1. Que ocurria.
2. Por que ocurria.
3. Como se soluciono.
4. Como validaron que quedo funcionando.
