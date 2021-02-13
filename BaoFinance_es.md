# Bao Finance
包子金钱

<hr/>

_Advertencia: Bao Finance está en alfa, no ha sido auditado y originalmente fue desarrollado por un equipo de una persona autodidacta. Estamos en el proceso de escalar el equipo, por favor sea consciente de los riesgos y use el producto en consecuencia._


Es como SNX + Aave, pero para Uniswap, Sushiswap y Balancer.

En lugar de reinventar la rueda Bao crea nuevas capacidades para protocolos existentes.

El token BAO actúa como un token de gobierno para el proyecto que está totalmente administrado por la comunidad. También está respaldado por el fondo de seguro donde llegan todas los cobros de Bao.

<hr/>

## ¡Finanzas envueltas deliciosamente!

Bao (包) significa tesoro o paquete. Algo maravilloso envuelto en otra capa. Los bollos Bao, o en chino Baozi (包子) son deliciosas albóndigas envueltas.

Estos bollos bao reflejan la tradición de tomar algo bueno que existe, y envolverlo para crear un nuevo tesoro.

Bao Finance apunta a lograr esto siendo un nuevo protocolo que agrega características a sistemas DeFi existentes.


Bao Finance actualmente planea agregar:

* Cultivo de rentabilidad (_Yield farming_) **[¡Hecho!]**
* Cultivo de rentabilidad con tokens LP de Sushi y Balance.
* Activos sintéticos a Uniswap usando tokens UniV2-LP.
* Activos sintéticos a Sushiswap usando tokens Sushi LP.
* Activos sintéticos a Balancer usando tokens Balancer Pool.
* Transar márgenes (_margin trading_) y órdenes limitadas (_limit orders_) a Uni/Sushi, basadas en tokens LP colocados. (_staked_)
* Pozos para préstamos (_lending pools_) creados con tókenes Uni/Sushi.
* Opciones/Futuros perpetuos a Uni/Sushi basados en tokens LP colocados.
* Sistemas de auto-balance para que los usuarios puedan balancear sus activos sintéticos, futuros y tokens LP.

Por ello, BAO significa "balance, automatización y opciones".

<hr/>

## ¿Dónde comenzamos?

Bao Finance se enfoca primero en proveer una distribución temprana justa, y luego en la creación de activos sintéticos.

### Distribución

Para nuestra distribución usaremos una versión modificada de la infraestructura de cultivo de SushiSwap.

Ya que Bao Finance no intenta crear su propio competidor para Uniswap, no habrá migración a pozos propios. En su lugar, se usará el método de cultivo de rentabilidad para la distribución.

Hemos realizado un número de cambios al sistema de distribución con el fin de:

* Prevenir abusos/aprovechamientos de préstamos instantáneos (_flash loans_) y acuñación instantánea (_flash minting_).
* Incentivar la participación a largo plazo en el sistema.
* Crear una tesorería robusta y diversa.
* Crear fondos de tesoro adicionales que la pertenezcan a la comunidad.
* Penalizar usuarios que dejan los pozos demasiado rápido y que intentan manipular precios u optimizar el cultivo.
* Crear bloqueos y consolidaciones para reducir la deflación y alinear a los participantes a largo plazo.

Puede leer mas sobre estos cambios en nuestra "página de distribución".

### Activos sintéticos

Los activos sintéticos son parte importante en un ecosistema descentralizado. Permiten una infraestructura descentralizada que ofrece activos que siguen los precios de cualquier sistema.

Esto quiere decir que los usuarios podrían hacer activos sintéticos que sigan el precio de BTC, o el inverso del precio de BTC (creando un _put_ sintético). También significa que puedes seguir precios de acciones u otros activos tradicionales, permitiendo a los usuarios alrededor del mundo tener acceso confiable, descentralizado, 24 x 7, a acciones como $AAPL.

Ahora mismo los protocolos para sintéticos existentes (como Synthetix y UMA) requieren que ponga sus activos en un token base para colateralizar la creación de su activo sintético, tomando riesgo y perdiendo la exposición al activo subyacente de su elección.

En lugar de ello, permitimos a los usuarios proveer sus propios tokens Uniswap para crear activos sintéticos, de forma que conserven la exposición a los activos subyacentes y las tarifas LP de ese par transado.

A pesar de las ineficiencias del mercado para sintéticos en Ethereum, ya va por una capitalización de mercado (_market cap_) superior a los $1000M, y $1000M de valor total bloqueado (_TVL_).

Creemos que BAO incrementará esto dramáticamente haciendo que la creación de activos sintéticos sea algo práctico.



