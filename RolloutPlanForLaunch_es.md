# Plan de Lanzamiento

_Esta página describe el plan de lanzamiento propuesto actualmente._

1. Publicaremos un contrato "Timelock" basado en el _Compound Timelock_.
2. Lanzaremos el lote de desbloqueo inicial de Bao que estará en el fondo de recompensa.
  1. En lugar de 72 mil millones (7,2x10<sup>10</sup>), basándonos en decisiones de la comunidad bajaremos este monto a 40 mil millones (4x10<sup>10</sup>).
  2. 5 mil millones (5x10<sup>9</sup>) se desbloquearán de inmediato como recompensas. Los restantes 35 mil millones (3,5x10<sup>10</sup>) se pondrán en un _stream_ de Sablier.Finance y serán emitidos por 2 semanas. Esto es para prevenir el riesgo de un _dumping? de desarrollo hasta que tengamos una configuración _multisig_. Esto quiere decir que el fondo de la recompensa desbloqueada será de un máximo de 10% de la emisión en las primeras 3 semanas, en lugar de 30%.
3. Luego de ésto, nos aseguraremos que todas las variables del contrato "BaoToken.sol" estén fijadas, y cuando esto esté hecho la propiedad de "BaoToken.sol" será transferida a "BaoMasterFarmer.sol" esto es para prevenir que el desarrollador tenga mas control sobre las funciones de acuñación y bloqueo.
4. Una vez listo haremos que nuestro contrato "Timelock.sol" sea dueño de "BaoMasterFarmer.sol" lo que significa que las transacciones futuras necesitarán pasar por un mínimo de 48 horas antes de que se lleven a cabo.

Riesgos:

* Si cualquier variable de configuración se olvida entonces el lanzamiento se retrasará al menos 48 horas pues no hay forma de actualizar las variables mas rápido.
* Si hay errores o bugs el desarrollador no podrá corregirlas al menos por 48 horas.
* Si hay algun hack el desarrollador no podrá migrar al menos por 48 horas y los usuarios serán forzaros a girar. Girar en tan poco tiempo conlleva una gran tarifa. Si esto pasa el desarrollador retornará las tarifas de giro pero si hay muchos usuarios esto tomará tiempo para llevarse a cabo.

Poner el contrato tras un timelock lo mantiene seguro de riesgos de _rugpull_ pero hace mas difícil responder a errores y problemas bloqueantes.


Los miembros de la comunidad debe estar muy conscientes de los riesgos que vienen con el lanzamiento.

Si no puede tolerar estos riesgos, se aconseja que no ponga sus activos en el pozo durante el lanzamiento y en lugar espere hasta que el contrato esté mas probado.
