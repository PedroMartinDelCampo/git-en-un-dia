# El primer repositorio

Antes de crear el primer repositorio con Git, se debe configurar algunos detalles. Para ello se utiliza el comando`git config`. Hay diferentes opciones para éste comando, por ejemplo, para asignar variables se usa la siguiente sintáxis:

```bash
git config [scope] <key> <value>
```

Donde scope es el alcance de la configuración \(ver Tabla 5.1\), key es el nombre de la variable y value su valor. A continuación se muestra cómo configurar el nombre y correo que aparecen al colaborar en un proyecto, así como el editor que se utilizará para editar comentarios acerca de los cambios hechos.

```
git config --global user.email "pedro.martin@lkmx.io"
git config --global user.name "Pedro Martín del Campo González"
git config --global core.editor "nano"
```

Hay muchas otras variables, pero para iniciar es suficiente.

**Tabla 5.1 Alcances**

| **Alcance** | **Descripción** |
| --- | --- |
| --global | Aplica a todos los repositorios del usuario actual |

