# Consideraciones generales

1. Cada integrante del equipo cuenta con una _branch_ personal.
2. Existe una _branch_ general ‘main’ donde se encuentra la versión definitiva del proyecto.
3. Cualquier contribución debe ser efectuada en la _branch_ personal del contribuyente para posteriormente ser integrada a la _branch_ de desarrollo ‘dev’.
4. Todos los integrantes pueden efectuar _commits_ en cualquier momento, pero sólo el líder del área puede hacer _merge_. 
5. Debe de haber aprobación de una mayor parte de los miembros del equipo de trabajo para realizar un _merge_ a la _branch_ general ‘main’.
6. Cada _commit_ debe de ir acompañado con un título y descripción breve sobre los cambios realizados. 
7. En caso de existir la participación de múltiples integrantes dentro de un _commit_ se incluyen todos los nombres en la sección de detalles.


# Formatos para contribuciones

## Commits

### Estructura de un Commit
Los _commits_ deben seguir la siguiente estructura: `<TIPO>: (<ALCANCE>) <MENSAJE>`
1. **Tipo**: Describe en una palabra lo que se hizo en el _commit_, por ejemplo `fix` cuando se resolvió un error (Ver esta [tabla](#tipos-de-commits) como referencia).
2. **Alcance [opcional]**: Se pone entre paréntesis y se refiere a qué parte de la aplicación se ve afectada por el _commit_, por ejemplo `(Button)`.
3. **Mensaje**: Descripción breve de lo implementado. Es importante considerar lo siguiente de los mensajes:
> [!TIP]
> Para escribir un mejor mensaje, es recomendable tomar las siguientes consideraciones:
> - Ser claro y conciso.
> - Utilizar verbos imperativos al inicio del mensaje. Por ejemplo: `Agregar`, `Actualizar`, etc.
> - Utilizar menos de 50 caracteres.

### Tipos de Commits
|**Tipo** | **Descripción**
-- | --
feat | Nuevas características
fix | Corrección de errores
build | Cambios en el sistema de compilación
chore | Cambios que no afectan el entorno de producción
docs | Cambios en la documentación
perf | Mejoras en el rendimiento
revert | Reversiones a un _commit_ anterior
style | Cambios en la sintaxis
test | Agregar o corregir tests

### Ejemplos
- Feat: (Reservaciones) Agregar botón para cancelar reservación
- Style: (Login) Alinear colores con paleta de la empresa

## Pull Requests

### Estructura de un Pull Request
```
## Descripción de cambios
<!--- Descripción en formato de viñetas -->

## Error que resuelve o característica que se implementa
<!--- Número y enlace -->

## Lista de Verificación
- [ ] Revisé a detalle mi código.
- [ ] Si se trata de una característica esencial, he realizado las pruebas correspondientes.
- [ ] Agregué comentarios a mi código.
- [ ] Mis cambios no generan ninguna alerta.
```

### ¿Cómo referenciar un error o característica?
> [!IMPORTANT]
> Para poder referenciar un error o característica, es necesario primero definir un _issue_. Se puede definir un _issue_ en la sección **Issues** > **New Issue** o dando click [aquí](https://www.example.com/).
1. Vista la sección de [Issues](https://www.example.com/) para comprobar el índice del _issue_ que se resolvió.
2. Escribir `#` seguido del índice del _issue_. Por ejemplo: `#235`

### Ejemplo
> [!NOTE]
> El enlace a los issues no se puede visualizar en las páginas de la wiki.

#### Descripción de cambios
- Agregar botón para cancelar reservación
- Agregar endpoint al API para cancelar reservación

#### Error que resuelve o característica que se implementa
- [Issue #43504](https://www.example.com/)

#### Lista de Verificación
- [X] Revisé a detalle mi código.
- [X] Si se trata de una característica esencial, he realizado las pruebas correspondientes.
- [X] Agregué comentarios a mi código.
- [X] Mis cambios no generan ninguna alerta.
