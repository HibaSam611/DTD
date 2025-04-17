<!--
Nombre: Hiba Samraoui Samraoui
Curso: 1ºDAM
Fecha: 14/04/2025
Ejercicio: 3 - Expresiones regulares
-->

1. Capítulo con 1 dígito:
   - `"Capítulo \d"`
   - `"Capítulo [0-9]"`

2. Capítulo con 1 o 2 dígitos:
   - `"Capítulo \d{1,2}"`
   - `"Capítulo [0-9]{1,2}"`

3. Capítulo sin el 0 inicial:
   - `"Capítulo [1-9][0-9]?"`
   - `"Capítulo [1-9]\d?"`

4. Capítulo con uno o más dígitos:
   - `"Capítulo \d+"`
   - `"Capítulo [0-9]{1,}"`

5. Cualquier primer carácter no dígito + "Z":
   - `\D{1}Z`
   - `[^0-9]Z`

6. AB seguido de 2 o más B y una C:
   - `"AB{2,}C"`
   - `"ABB+B*C"`

7. "R" seguido de 2+ "S" y opcional [3-8]:
   - `"RS{2,}[3-8]?"`
   - `"RS{2,}(3|4|5|6|7|8)?"`

8. "COD" + 3 dígitos + 1+ cualquier carácter:
   - `"COD\d{3}.+"`
   - `"COD[0-9]{3}.+"`
