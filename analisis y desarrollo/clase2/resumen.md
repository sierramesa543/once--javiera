# Resumen: Requerimientos, Calidad e Historias de Usuario

## Requerimientos

Un requerimiento es una propiedad documentada y verificable que un sistema debe poseer para resolver un problema o alcanzar un objetivo. Para ser considerado un requerimiento debe poder escribirse y comprobarse.

### Niveles de abstracción

1. **Necesidad del usuario:** expresa lo que el usuario necesita.
2. **Requerimiento del sistema:** describe lo que el sistema debe hacer.
3. **Especificación técnica:** detalla cómo se implementará técnicamente.

---

## Requerimientos Funcionales (RF)

Describen las acciones o funciones que el sistema debe realizar. Indican **qué hace el sistema**.

### Características

* Utilizan verbos de acción como registrar, calcular, mostrar o validar.
* Definen entradas, salidas y reglas de decisión.
* Se redactan normalmente como:
  *"El sistema deberá..."*

### Categorías principales

* Autenticación.
* Cálculo.
* Persistencia de datos.
* Comunicación.
* Reportes.
* Validación.

---

## Requerimientos No Funcionales (RNF)

Describen **cómo debe comportarse el sistema** y las condiciones de calidad que debe cumplir.

### Categorías principales

* Rendimiento.
* Seguridad.
* Usabilidad.
* Confiabilidad.
* Escalabilidad.
* Mantenibilidad.
* Portabilidad.
* Cumplimiento legal.

Un RNF debe ser medible, indicando una métrica, un valor objetivo y una forma de verificación.

---

## Atributos de Calidad

Son características generales que determinan la calidad del software. Según la norma ISO/IEC 25010 existen ocho atributos principales:

1. Adecuación funcional.
2. Eficiencia de desempeño.
3. Compatibilidad.
4. Usabilidad.
5. Confiabilidad.
6. Seguridad.
7. Mantenibilidad.
8. Portabilidad.

Los atributos representan conceptos generales, mientras que los RNF son su aplicación concreta y medible.

---

## Historias de Usuario

Son descripciones breves de una necesidad desde la perspectiva del usuario.

### Estructura

**Como** [tipo de usuario],
**quiero** [funcionalidad],
**para** [beneficio].

### Reglas INVEST

* Independiente.
* Negociable.
* Valiosa.
* Estimable.
* Pequeña.
* Testeable.

### Criterios de aceptación

Permiten verificar que la historia está completa y suelen escribirse con el formato:

* Dado...
* Cuando...
* Entonces...

## Conclusión

Los requerimientos son la base del desarrollo de software. Los requerimientos funcionales definen qué hace el sistema, los no funcionales establecen la calidad con la que debe hacerlo, los atributos de calidad permiten evaluar el software y las historias de usuario ayudan a expresar las necesidades de manera clara y centrada en el usuario.
