# Planificador de Estrellas Primarias (Sword x Staff)

Calculadora bilingüe (ES/EN) de Estrellas Primarias (Primo Stars) para Sword x Staff. Todo vive en un solo archivo: `index.html`.

- **Publicada en:** https://claude.ai/artifact/AziWcNbpUkYWBR2Lvbtnw6 (compartida con «cualquiera con el enlace»).
- **Probarla en tu PC:** abre `index.html` con doble clic, o sírvela con `python -m http.server 8768` dentro de esta carpeta y entra a http://localhost:8768.
- **Publicar cambios:** edita `index.html` y pídele a Claude que lo vuelva a publicar en el mismo enlace del Artifact. Si la sesión es nueva, pásale el enlace.

## Qué hace

- Pestañas: Mi meta, Temporada, Personaje, Niveles, Materiales, Reinos y Pagos (opcional).
- Arma un plan con 3 escenarios:
  1. **Tu meta.**
  2. **Tu meta realista:** lo máximo que alcanzas con todo lo que tendrás hasta el cierre.
  3. **Gasta hoy y ahorra desde hoy:** gastas solo lo que ya tienes guardado y ahorras el resto para la próxima temporada. Es el número grande del panel.
- **Pacto Astral (v47):** la meta se elige de una lista de hitos o se escribe a mano.
  - Si el número que pones no es un hito, te avisa y te propone el hito anterior y el siguiente.
  - Cada escenario muestra el último premio que alcanzas y cuánto falta para el próximo.
  - Hay una tabla con todos los hitos.
- **Gastar hoy vs guardar (v48):** en el escenario 3 compara las estrellas que ganas gastando hoy con las que valdrían esos mismos materiales en la T siguiente como un rango: el más alto usa los materiales apenas pasas el piso de la T siguiente; el más bajo, al final, si subes lo mismo que en esta temporada (allá cada nivel cuesta más pero también da más puntos). Las entradas de Reinos cuentan con su rendimiento de la T siguiente, nivel más bajo.
- **Clasificación:** cada escenario muestra la Valoración de Progreso al cierre. La Clasificación de Valoración de Temporada suma Jugabilidad + Progreso + Equipamiento, y la calculadora solo mide Progreso.

## Datos del juego confirmados (con capturas del usuario)

- **Cierre de temporada** (confirmado por jugadores en el Discord oficial, 2026-10-09):
  - Se borran los niveles de personaje, fantomons, equipamiento y reliquias por encima de 100. Lo gastado en ellos no vuelve.
  - La T2 empieza en Lv100: hay que subir de 100 a 130 sin ganar puntos.
  - Los materiales y las herramientas de Reinos que no gastes pasan a la temporada siguiente. Los jugadores recomiendan guardar las herramientas.
  - En la calculadora, los niveles de 101 a 130 se pagan en la T2 con los costos de la T1 (estimado: las tablas del juego empiezan en el piso de cada temporada).

- **Fórmula T1:** puntos = Σ(niveles por encima de 100 × peso).
  - Pesos: personaje 100, equipamiento 38, reliquia 57 (piso 10), habilidad 13, fantomon 14.
  - Estrellas = puntos ÷ 100 + 10 fijas + las de temporadas anteriores.
  - Verificado: 14.089 puntos = 150 estrellas.
  - El personaje cuenta la fracción de nivel que lleva: 24,39 niveles = 2.439 puntos.
- **Reinicio diario:** 8:00 UTC-5 (9:00 en Venezuela).
- **Reinos:** 20 compras por día en cada Reino; cada compra da 5 entradas y cuesta 100. Las misiones diarias dan 5 entradas de cada Reino.
- **Carro y Cama:** guardan como máximo 36 h de producción. El Carro da calidad común (gris).
- **Pacto Astral:**
  - Las estrellas se gastan al cerrar la temporada y se acumulan de una temporada a otra.
  - Hitos: 5…40 (cada 5), 48…104 (cada 8), 116…200 (cada 12), 215…320 (cada 15), 340…480 (cada 20), 505…680 (cada 25), 710…860 (cada 30). Por encima de 860 no está confirmado.
  - Los premios se repiten en este orden desde el hito 5: ATQ +1%, Mazmorra: Aparición de Equipamiento +3%, DEF +1%, Aparición de Gemas +5%, PS +1%, Mazmorra: Recompensas de Valoración ×2 +2%, VEL +1%, Obtención de EXP +2%.

## Fuentes

- Reglas por temporada, tablas de EXP y costos: planificador de 0xNobody (https://0xnobodyyt.github.io/sxs-primo-calculator/), con crédito en la página.

## Pendiente

- Confirmar los topes de habilidad y fantomon en la T1.
- Confirmar los nombres de los objetos en inglés.
- Confirmar los costos de la T6 en adelante.
- Confirmar los hitos del Pacto por encima de 860.
- Confirmar que los niveles de 101 a 130 cuestan en la T2 lo mismo que en la T1.
