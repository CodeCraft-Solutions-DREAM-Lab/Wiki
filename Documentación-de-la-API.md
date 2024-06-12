**Puedes consultar la documentación y realizar pruebas de las peticiones directamente en nuestra [documentación interactiva 📑](https://dreamlab-api.azurewebsites.net/docs/).**

<!-------------------------------------- AUTH -------------------------------------->
## Auth
$${\color{lightgreen}POST}$$
```
/auth/usuario
```
```
/auth/token
```

<!-------------------------------------- CORRER ASIGNACIÓN -------------------------------------->
## Correr asignación
$${\color{lightblue}GET}$$
```
/correr-asignacion
```

<!-------------------------------------- DASHBOARD -------------------------------------->
## Dashboard
$${\color{lightblue}GET}$$
```
/dashboard/reservacionesByMes
```
```
/dashboard/reservacionesBySalaByMes
```
```
/dashboard/salasDisponibles
```
```
/dashboard/usoMaterialByMes
```
```
/dashboard/penalizacionesByMes
```

<!-------------------------------------- ESTATUS -------------------------------------->
## Estatus
$${\color{lightblue}GET}$$
```
/estatus
```

<!-------------------------------------- EXPERIENCIAS -------------------------------------->
## Experiencias
$${\color{lightblue}GET}$$
```
/experiencias/
```
```
/experiencias/expertienciasActivas
```
```
/experiencias/autodirigidas
```
```
/experiencias/{id}
```
$${\color{lightgreen}POST}$$
```
/experiencias/UFs
```
```
/experiencias/crear
```

<!-------------------------------------- LOGROS -------------------------------------->
## Logros
$${\color{lightgreen}POST}$$
```
/logros/progresoLogro/{idUsuario}/{idLogro}
```
$${\color{orange}PUT}$$
```
/logros/{idUsuario}/{idLogro}
```

<!-------------------------------------- MATERIALES -------------------------------------->
## Materiales
$${\color{lightblue}GET}$$
```
/materiales
```
```
/materiales/recomendados
```
```
/materiales/bySala
```

<!-------------------------------------- MESAS -------------------------------------->
## Mesas
$${\color{lightblue}GET}$$
```
/mesas
```
```
/mesas/{idSala}
```

<!-------------------------------------- PERFIL -------------------------------------->
## Perfil
$${\color{lightblue}GET}$$
```
/perfil/logros/{idUsuario}
```
```
/perfil/{idUsuario}
```
$${\color{lightgreen}POST}$$
```
/perfil/logros/{idUsuario}
```

<!-------------------------------------- RESERVACIONES -------------------------------------->
## Reservaciones
$${\color{lightblue}GET}$$
```
/reservaciones
```
```
/reservaciones/cronograma
```
```
/reservaciones/cronogramaSingle/{idReservacion}
```
```
/reservaciones/cronograma/{id}
```
```
/reservaciones/usuario/{id}
```
```
/reservaciones/{id}
```
$${\color{lightgreen}POST}$$
```
/reservaciones
```
```
/reservaciones/cancelar
```
```
/reservaciones/ultimas
```
$${\color{orange}PUT}$$
```
/reservaciones/{id}
```
$${\color{red}DELETE}$$
```
/reservaciones/{id}
```

<!-------------------------------------- RESERVACIONES MATERIALES -------------------------------------->
## Reservaciones materiales
$${\color{lightgreen}POST}$$
```
/reservaciones-materiales/changeEstatus
```

<!-------------------------------------- SALAS -------------------------------------->
## Salas
$${\color{lightblue}GET}$$
```
/salas
```
```
/salas/salasActivas
```
```
/salas/cronograma
```
```
/salas/{id}
```
```
/salas/nameFromExperienceId/{id}
```
$${\color{lightgreen}POST}$$
```
/salas/horasLibres
```
$${\color{orange}PUT}$$
```
/salas/cambiarEstadoSalas
```

<!-------------------------------------- UFs -------------------------------------->
## Unidades de formación
$${\color{lightblue}GET}$$
```
/ufs
```

<!-------------------------------------- USUARIOS -------------------------------------->
## Usuarios
$${\color{lightblue}GET}$$
```
/usuarios
```
```
/usuarios/nombreUsuario/{tagID}
```
$${\color{lightgreen}POST}$$
```
/usuarios/cambiarPrioridad
```
$${\color{orange}PUT}$$
```
/usuarios/{idUsuarios}
```

<!-------------------------------------- VIDEOWALL -------------------------------------->
## Videowall
$${\color{lightblue}GET}$$
```
/videowall/reservaciones
```
