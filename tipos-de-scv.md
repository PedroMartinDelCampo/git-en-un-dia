# Tipos de SCV

La forma de trabajar varía entre un SCV y otro, pero en general se les puede clasificar como Locales, Centralizados y Distribuidos, los cuales se mencionan a continuación.

## Locales

Éstos SCV fueron los primeros en surgir, y aún están instalados por defecto en algunas máquinas \(por ejemplo, rcs en Mac\). Su función es sustituir los respaldos hechos manualmente por archivos llamados parches, que guardan los cambios hechos por el usuario, y el SCV entonces puede revertir o volver a aplicar el parche.

Éstos SCV efecticamente removieron la necesidad de crear respaldos con cada cambio, lo cual malgasta el espacio en la memoria y es demasiado susceptible, pero con el auge del internet vino una nueva necesidad: colaborar con otros compañeros de trabajo. Además, si el repositorio se dañaba, no había forma de recuperarlo.

## Centralizados

Los SCV's centralizados proveen la capacidad de colaborar con un gran número de compañeros. Su principal característica es que el historial del proyecto está en un servidor central \(de ahí su nombre\), y todos los colaboradores trabajan en éste único repositorio a través de internet. Ésto implica que no existe acceso al SCV si no hay internet \(y el acceso es lento y depende de la latencia de la conexión a internet\), y que a menos que se hagan respaldos frecuentes \(lo cual nos lleva de vuelta al inicio\) no hay forma de recuperar el historial si éste se daña. En otras palabras, aún existe un único punto de quiebre.

## Distribuidos

Tomando en cuenta lo anterior, los SVC's distribuidos son de cierta forma un híbrido entre los centralizados y locales. El historial puede compartirse como en los centralizados, pero de una forma muy distinta. La principal diferencia es que el colaborador no trabaja directamente con el historial central, sino que lo clona en su máquina, de manera que prácticamente todas las operaciones son locales \(excepto cuando se desea compartir el trabajo\).

Aunque puede parecer algo sencillo, ésto trae bastantes ventajas. Por ejemplo, no se necesita internet para trabajar o acceder al historial, y si el servidor se daña, cualquier colaborador puede compartir su historial con el servidor sin perder prácticamente nada.

