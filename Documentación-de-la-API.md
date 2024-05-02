**Puedes consultar la documentación y realizar pruebas de las peticiones directamente en nuestra [documentación interactiva 📑](https://dreamlab-api.azurewebsites.net/docs/).**

<!-------------------------------------- AUTH -------------------------------------->
## Auth
### $${\color{lightgreen}POST}$$
```
/auth/usuario
```
```
/auth/token
```

<!-------------------------------------- CHATBOT -------------------------------------->
## Chatbot
### $${\color{lightgreen}POST}$$
```
/chatbot
```

<!-------------------------------------- EXPERIENCIAS -------------------------------------->
## Experiencias
### $${\color{lightblue}GET}$$
```
/experiencias
```
```
/experiencias/autodirigidas
```
```
/experiencias/{id}
```
### $${\color{lightgreen}POST}$$
```
/experiencias/UFs
```

<!-------------------------------------- LOGROS -------------------------------------->
## Logros
### $${\color{orange}PUT}$$
```
/logros/{idUsuario}/{idLogro}
```

<!-------------------------------------- MATERIALES -------------------------------------->
## Materiales
### $${\color{lightblue}GET}$$
```
/materiales-disponibles
```

<!-------------------------------------- MESAS -------------------------------------->
## Mesas
### $${\color{lightblue}GET}$$
```
/mesas
```
```
/mesas/{idSala}
```

<!-------------------------------------- PERFIL -------------------------------------->
## Perfil
### $${\color{lightblue}GET}$$
```
/perfil/logros/{idUsuario}
```
```
/perfil/{idUsuario}
```
### $${\color{lightgreen}POST}$$
```
/perfil/logros/{idUsuario}
```

<!-------------------------------------- RESERVACIONES -------------------------------------->
## Reservaciones
### $${\color{lightblue}GET}$$
```
/reservaciones
```
```
/reservaciones/usuario/{id}
```
```
/reservaciones/{id}
```
### $${\color{lightgreen}POST}$$
```
/reservaciones
```
### $${\color{orange}PUT}$$
```
/reservaciones/{id}
```
### $${\color{red}DELETE}$$
```
/reservaciones/{id}
```

<!-------------------------------------- SALAS -------------------------------------->
## Salas
### $${\color{lightblue}GET}$$
```
/salas
```
```
/salas/{di}
```
```
/salas/nameFromExperienceId/{id}
```
### $${\color{lightgreen}POST}$$
```
/salas/horasLibres
```

<!-------------------------------------- USUARIOS -------------------------------------->
## Usuarios
### $${\color{lightblue}GET}$$
```
/usuarios
```
### $${\color{orange}PUT}$$
```
/usuarios/{idUsuarios}
```

<!-------------------------------------- VIDEOWALL -------------------------------------->
## Videowall
### $${\color{lightblue}GET}$$
```
/videowall/reservaciones
```
