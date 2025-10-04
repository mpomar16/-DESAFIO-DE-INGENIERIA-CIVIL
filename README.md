# DESAFIO INGENIERIA CIVIL
**Métodos:** Inversa de `A`, **Jacobi**, **Gauss-Seidel**, **LU** (con pivoteo parcial) y **Gráfico 3D** de los planos + punto de intersección.

Sitio de una sola página (HTML + JS) para resolver sistemas lineales **3×3** típicos del ejercicio de canteras. Permite **ingresar datos**, usar **valores por defecto**, ajustar **tolerancia** y **máx. iteraciones**, y visualizar el **gráfico 3D**.

---

## 📄 Enunciado (consigna del ejercicio)
Un ingeniero civil requiere **4800**, **5810**, **5690** m³ de **arena**, **grano fino** y **grano grueso**, respectivamente.  
Determinar la cantidad de metros cúbicos que se debe transportar desde cada cantera para cumplir con sus requerimientos.

Resolver por:
- **INV(A) · b** (inversa de la matriz)
- **Jacobi** o **Gauss-Seidel**
- **LU** (con pivoteo parcial)

Además, **explicar la solución** y mostrarla **por código y por Excel**.

Composición por m³ de material de cada cantera (porcentaje → fracción). Esto define la matriz del sistema `A·x = b`:

```txt
A = [[0.52, 0.20, 0.25],
     [0.30, 0.50, 0.20],
     [0.18, 0.30, 0.55]]

b = [4800, 5810, 5690]
```
---

## 🎯 Características
- **Pestañas** por método: Inversa, Jacobi, Gauss-Seidel, LU y Gráfico 3D.
- **Entrada editable** de `A` (3×3) y `b` (3×1).
- **Botón “Cargar datos por defecto”** (ejercicio de canteras).
- **Parámetros iterativos**: tolerancia y máx. iteraciones (usados por Jacobi/Seidel).
- **Resultados amigables**:
  - `x` con 6 decimales.
  - **Interpretación** con m³ truncados por cada cantera.
  - (En Inversa/LU) `A⁻¹`, `L⁻¹` y `U⁻¹` desplegables.
- **Gráfico 3D** con los 3 planos e **intersección** etiquetada.
- **Auto-tests silenciosos** en consola para validar coherencia entre métodos.
