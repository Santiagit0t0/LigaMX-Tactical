# ⚽ LigaMX Tactical Engine

> Sistema de gestión de plantillas futbolísticas y motor de simulación táctica desarrollado en Java para la asignatura de **Programación Orientada a Objetos**.

---

## 👥 Integrantes del Equipo
* **Santiago**
* **Christopher**

---

## 📌 Descripción del Proyecto
`LigaMX Tactical Engine` es una aplicación desarrollada en Java (ejecutable por consola en BlueJ) diseñada para cuerpos técnicos y analistas de rendimiento deportivo. Permite administrar de forma dinámica la plantilla de un equipo de la Liga MX, evaluar el rendimiento de los futbolistas de acuerdo a su posición táctica y calcular el impacto del desgaste físico (fatiga) acumulado tras disputar minutos de juego.

---

## 🛠️ Pilares de POO Aplicados

* **Herencia:** Clase abstracta madre `Jugador` y subclases especializadas `Portero`, `Defensa` y `Delantero`.
* **Polimorfismo:** Implementación del método abstracto sobrescrito `resolverJugadaClave(int intensidad)` adaptado a las métricas específicas de cada posición.
* **Encapsulamiento:** Atributos privados restringidos con métodos getters y setters validados.
* **Colecciones Dinámicas:** Administración del plantel mediante `ArrayList<Jugador>` dentro de `ClubLigaMX`.
* **Manejo de Excepciones:** Control de errores de entrada y validaciones de rango mediante la excepción personalizada `DatoDeportivoInvalidException`.

---

## 📁 Estructura del Código

```text
src/
├── Jugador.java                        (Clase Abstracta Madre)
├── Portero.java                        (Clase Hija)
├── Defensa.java                        (Clase Hija)
├── Delantero.java                      (Clase Hija)
├── ClubLigaMX.java                     (Gestora de Plantilla)
├── Partido.java                        (Motor de Simulación y Fatiga)
├── DatoDeportivoInvalidException.java  (Excepción Personalizada)
├── MenuConsola.java                    (Interfaz de Usuario)
└── Main.java                           (Punto de Entrada)
