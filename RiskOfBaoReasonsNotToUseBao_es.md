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
* Dado que la migración tiene un bloque temporal, 
