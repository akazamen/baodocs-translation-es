# Riesgos de Bao / Razones para no usar Bao

Muchos equipos se enfocan en por que debería usar el producto que ellos hacen.

Pero en cripto DeFi, hay muchos riesgos y pensamos que es reponsable para un equipo decirle tales riesgos y razones por las cuales no usar el producto.

También destacamos pasos que tomamos para protección contra estos riesgos.

## Riesgos:

* "Bao Pendiente" (_Pending Bao_) es un balance pendiente. No está acuñado o bloqueado hasta que eliga cosechar. Si hay cambios en el contrato, que impacte los cálculos de Bao, o un pozo se vaya a la guillotina, si no cosecha los Bao pendientes no está acuñado y no puede ser reclamado. Los desarrolladores no tienen forma de anular estos cambios.
* Bao es un producto complicado. Si no se mantiene al día con el ecosistema o lee la documentación, puede perder sus "Baos Pendientes" durante los cambios. Estos cambios no impactarán Baos bloqueados o tokens LP.
* El nuevo sistema de depósito/giro podría tener errores matemáticos que resulten en fallas.
  * Hemos probado estas funciones, aplicando matemática segura, y las funciones parecen ser seguras pero siempre existe un riesgo. 
* Los deltas de bloque pueden tener errores o riesgo de no hacer los cálculos correctos, lo que podría impactar las tarifas de usuario.
* Una vez las tarifas se toman es muy difícil remapear estas tarifas de vuelta al usuario.
  * En todas las pruebas de delta de bloque y tarifas, se han tomado los montos correctos.
  * Tenemos comandos para ajustar manualmente los conteos de delta de bloque de forma que la atención a cliente pueda ayudar a usuarios enfrentando problemas.
* Casos de borde desconocidos no cubiertos en la lógica pueden causar errores de contrato.
* El sistema económico puede resultar en una distribución pesada que diluya demasiado el valor de los tokens para los usuarios iniciales.
  * Se recomienda siempre cultivar para Bao y no comprarlo como inversión (este no es un producto de inversión)
* Dado que la migración tiene un bloque temporal, si hay un error crítico o hackeo los usuarios deberán girar los tokens ellos mismos. Si esto pasa pueden tener tarifas mas altas del sistema de escala deslizante de tarifas.
* Los errores de _front end_ pueden romper la habilidad de interactuar con el contrato
  * Hemos documentado "Como usar manualmente el contrato"
* El equipo de Bao puede ser incapaz de entregar las etapas futuras del proyecto, si no retienen su talento técnico, enfrentan problemas financieros, o hay desafíos de gobernanza como ser votados fuera de forma temprana.
* El equipo Bao puede ser incapaz de entregar las etapas futuras del proyecto si hay cambios legales o regulatorios que lo demanden.
* Errores de _front end_ o de balance, pueden hacer muy difícil rastrear o distribuir de forma justa las recompensas para los usuarios que usen _referrals_.
* Los grandes inversionistas pueden dominar los pozos iniciales creando avances injustos en gobernanza o precios de mercado.
  * Hemos intentado mitigar esto agregando varios pozos diversos y recompensas y bloqueos de largo plazo que son malos para grandes proveedores de liquidez que buscan un proyecto de corto plazo.
* Las decisiones económicas tomadas por el equipo para proveer liquidez, pagar proveedores o pagar al equipo, pueden resultar en precio negativo de ecosistema durante los dias iniciales.
  * Esperamos balancear esto a largo plazo, razon por la cual los fondos de usuario están bloqueados y se consolidan durante 3 años.
* 
