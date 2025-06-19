---
applyTo: "**"
---

# Instrucciones para generación de código con Copilot

- Prioriza siempre la claridad y legibilidad del código sobre la optimización prematura.
- Añade comentarios explicativos en bloques de lógica compleja o poco intuitiva.
- Usa nombres descriptivos para variables, funciones y clases.
- Sigue las convenciones de estilo y formato del lenguaje y del proyecto (usa linters y formateadores si están disponibles).
- Si el proyecto tiene pruebas, sugiere o añade pruebas unitarias para nuevas funciones o cambios relevantes.
- Prefiere la reutilización de código existente antes de crear duplicados.
- Si usas dependencias externas, justifica su uso y referencia la documentación oficial.
- Para código asíncrono, maneja correctamente los errores y excepciones.
- Si el cambio afecta la seguridad, documenta los riesgos y mitigaciones.
- Si el código es experimental o tiene limitaciones conocidas, indícalo claramente en los comentarios.
- Cuando sea relevante, incluye ejemplos de uso en los comentarios o en la documentación.
- Si el código modifica la API pública, actualiza la documentación correspondiente.
- Usa el idioma predominante del proyecto para los nombres y comentarios.
- Si tienes dudas sobre requisitos o contexto, pide aclaraciones antes de asumir.

## Ejemplo de buenas prácticas en Python

```python
def calcular_area_circulo(radio: float) -> float:
    """
    Calcula el área de un círculo dado su radio.

    Args:
        radio (float): Radio del círculo.

    Returns:
        float: Área calculada.

    Raises:
        ValueError: Si el radio es negativo.
    """
    if radio < 0:
        raise ValueError("El radio no puede ser negativo")
    return math.pi * radio ** 2
```

## Ejemplo de buenas prácticas en JavaScript

```javascript
/**
 * Calcula el área de un círculo.
 * @param {number} radio - Radio del círculo.
 * @returns {number} Área calculada.
 * @throws {Error} Si el radio es negativo.
 */
function calcularAreaCirculo(radio) {
  if (radio < 0) throw new Error('El radio no puede ser negativo');
  return Math.PI * radio ** 2;
}
```

## Ejemplo de buenas prácticas en TypeScript

```typescript
/**
 * Calcula el área de un círculo.
 * @param radio Radio del círculo.
 * @returns Área calculada.
 * @throws Error si el radio es negativo.
 */
export function calcularAreaCirculo(radio: number): number {
  if (radio < 0) throw new Error('El radio no puede ser negativo');
  return Math.PI * radio ** 2;
}
```

## Ejemplo de buenas prácticas en SQL

```sql
-- Consulta para obtener usuarios activos
SELECT id, nombre, email
FROM usuarios
WHERE activo = TRUE;
```

## Ejemplo de buenas prácticas en Bash

```bash
# Script para hacer backup de una carpeta
SRC="/ruta/origen"
DEST="/ruta/destino"
tar -czf "$DEST/backup_$(date +%F).tar.gz" "$SRC"
```

## Consideraciones adicionales

- Si el código es para automatización de tareas, documenta claramente los parámetros y el flujo.
- Si el código es para infraestructura (Docker, Terraform, etc.), sigue las mejores prácticas de seguridad y portabilidad.
- Si el código es para frontend, prioriza la accesibilidad y la experiencia de usuario.
- Si el código es para backend, prioriza la robustez, manejo de errores y validaciones.
- Si el código es para machine learning, documenta los supuestos y limita el uso de datos sensibles.
- Si el código es para scripts de migración, asegúrate de que sea idempotente y reversible.
- Si el código es para pruebas, cubre casos límite y documenta los escenarios probados.
