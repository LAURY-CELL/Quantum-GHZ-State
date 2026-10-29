# Quantum-GHZ-State

Este repositorio contiene la simulacion cuántica de un **Estado GHZ (Greenberger-Horne-Zeilinger)** utilizando el entorno **Qiskit** de IBM y Python.

---

## Estructura del Circuito 
El circuito consta de 3 cúbits y 3 bits clásicos ('QuantumCircuit(3, 3)' ):

* **'h(0)'**: Aplica una compuerta **Hadamar** en el cúbit 0 para ponerlo en superposición.
* **'cx(0, 1)' y 'cx(1, 2)'**: Crean un entrelazamiento en cadena (efecto dominó) mediante compuertas CNOT consecutivas.
* **'measure(,)'**: Mapea en paralelo el colapso de los 3 cúbits a sus registros clásicos correspondientes.

---

## Resultados Estadisticos 
Al ejecutarse en 'AerSimulator' con 1024 *shots*, el sistema colapsa únicamente en estados de correlación cuántica perfecta:
* **Estado 000** : 525 conteos (51.2%)
* **Estado 111** : 499 conteos (48.8%)

* Nota: La ausencia total de otras combinaciones  (como '010' o '101') validan experimentalmente el entrelazamiento multipartito.*

---
