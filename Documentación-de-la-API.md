Puedes consultar la documentación y realizar pruebas de las peticiones directamente en nuestra [documentación interactiva](https://dreamlab-api.azurewebsites.net/docs/).

<!-------------------------------------- AUTH -------------------------------------->
## Auth
### POST
```
/auth/usuario
```
```
/auth/token
```

<!-------------------------------------- CHATBOT -------------------------------------->
## Chatbot
### POST
```
/chatbot
```

<!-------------------------------------- EXPERIENCIAS -------------------------------------->
## Experiencias
### $${\color{lightgreen}GET}$$
```
/experiencias
```
```
/experiencias/autodirigidas
```
```
/experiencias/{id}
```
### POST
```
/experiencias/UFs
```

<!-------------------------------------- LOGROS -------------------------------------->
## Logros
### PUT
```
/logros/{idUsuario}/{idLogro}
```

<!-------------------------------------- MATERIALES -------------------------------------->
## Materiales
### $${\color{lightgreen}GET}$$
```
/materiales-disponibles
```

<!-------------------------------------- MESAS -------------------------------------->
## Mesas
### $${\color{lightgreen}GET}$$
```
/mesas
```
```
/mesas/{idSala}
```

<!-------------------------------------- PERFIL -------------------------------------->
## Perfil
### $${\color{lightgreen}GET}$$
```
/perfil/logros/{idUsuario}
```
```
/perfil/{idUsuario}
```
### POST
```
/perfil/logros/{idUsuario}
```

<!-------------------------------------- RESERVACIONES -------------------------------------->
## Reservaciones
### $${\color{lightgreen}GET}$$
```
/reservaciones
```
```
/reservaciones/usuario/{id}
```
```
/reservaciones/{id}
```
### POST
```
/reservaciones
```
### PUT
```
/reservaciones/{id}
```
### DELETE
```
/reservaciones/{id}
```

<!-------------------------------------- SALAS -------------------------------------->
## Salas
### $${\color{lightgreen}GET}$$
```
/salas
```
```
/salas/{di}
```
```
/salas/nameFromExperienceId/{id}
```
### POST
```
/salas/horasLibres
```

<!-------------------------------------- USUARIOS -------------------------------------->
## Usuarios
### $${\color{lightgreen}GET}$$
```
/usuarios
```
### PUT
```
/usuarios/{idUsuarios}
```

<!-------------------------------------- VIDEOWALL -------------------------------------->
## Videowall
### $${\color{lightgreen}GET}$$
```
/videowall/reservaciones
```
