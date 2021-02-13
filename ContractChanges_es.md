# Cambios en el Contrato

Muchos están familiarizados con protocolos de cultivo de rentabilidad incluyendo Yam, Sushi y Lua.

Muchos pueden esperar que Bao siga los mismos exactos patrones de estos sistemas.

Acá por transparencia deseamos destacar algunos cambios clave que este sistema tiene.

## Módulo de autorización

<=== CODE HERE: contract Authorizable is Ownable... ===>

El módulo de autorización es una extensión del módulo Ownable que es estándar para los contratos ECR-20.

Esto nos permite crear una lista de monederos (_wallet_) aprobados que pueden realizar comandos específicos como si fueran dueños. Hicimos esto por que el contrato BaoMasterFarmer debe ser un dueño del contrato de Bao Token, pero en el futuro desearemos migrar esto a nuevos contratos tales como contratos de activos sintéticos. 

El módulo de autorización se usa solo en reclamar posesión y acuñar la emisión inicial de tokens para alimentar (_seed_) al ecosistema.

## Módulo Timelocker

Similar al módulo de autorización, también hemos creado un status "Timelocker" (bloqueo temporal).

El status Timelocker bloquea la migración (y solo la migración) de modo que siempre necesita pasar a través del contrato de timelock.

# Sistema de Bloqueo (_Locking_)

A diferencia de distribuciones Sushi, agregamos el concepto de "bloqueo" cuando un usuario gana un token bao, 95% queda bloqueado y distribuído por un períódo de 3 años.

El fondo de desarrollo y de fundadores tiene el mismo bloqueo.

Los bloqueos no comienzan a liberarse hasta luego de un año, y despues se desbloquean linealmente, en cada bloque, durante 3 años.

Esto quiere decir que mientras los usuarios puedan ganar sus bao de forma temprana, se consolidarán en el tiempo tal como lo hacen los equipos para crear usuarios harmoniosos que estén alineados con las metas de la comunidad.

Debido a que el bloqueo de token es parte nativa del token bao, quiere decir que una bez un usuario lo gana el Equipo Bao **no puede** remover el token del usuario. Es parte de su posición incluso si está bloqueado. Podrá ser reclamado y usado una vez el _timelock_ expire.

<=== CODE HERE: function canUnlockAmount(address _holder) public view returns (uint256)... ===>

## Deltas de Bloque y Sistema de Tarifas/Penalidades

Como parte de cada objeto de usuario, incluimos un rastreo de bloques de depósito y giro.

Esto nos permite rastear el tiempo entre depósitos y giros, usando esto para nuestro sistema de tarifas 
