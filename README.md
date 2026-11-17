# Unbrewed heroes

Mazos de Unmatched (Restoration Games) en el formato nativo de [Unbrewed](https://unbrewed.xyz),
para partidas privadas. El arte es de Restoration Games.

## Importar en Unbrewed

En **unbrewed.xyz/bag**, pega un enlace en la barra de añadir.

**Una caja entera de una vez:**

| Caja | Enlace |
|---|---|
| Cobble & Fog | `https://raw.githubusercontent.com/alexkhudov2002/Unmatched/main/cobble-fog.json` |

**Héroes sueltos:**

| Héroe | Enlace |
|---|---|
| Sherlock Holmes | `https://raw.githubusercontent.com/alexkhudov2002/Unmatched/main/sherlock-holmes/sherlock-holmes.json` |
| Dracula | `https://raw.githubusercontent.com/alexkhudov2002/Unmatched/main/dracula/dracula.json` |
| Invisible Man | `https://raw.githubusercontent.com/alexkhudov2002/Unmatched/main/hombre-invisible/hombre-invisible.json` |
| Jekyll & Hyde | `https://raw.githubusercontent.com/alexkhudov2002/Unmatched/main/jekyll-hyde/jekyll-hyde.json` |

Si un mazo cambia, bórralo de la bolsa y vuelve a añadirlo: Unbrewed guarda una copia en el navegador.

## Fichas en la mesa

- **Sherlock** (con Watson) y **Dracula** (con 3 Sisters): Unbrewed pone las fichas de los luchadores
  en la esquina de cada jugador, con la vida enlazada.
- **Invisible Man**: su ficha y las 3 fichas de niebla.
- **Jekyll & Hyde**: su ficha y la de transformación, que se gira entre Dr. Jekyll y Mr. Hyde.

Estos dos últimos usan una lista de fichas guardada en el mazo, y Unbrewed la pone siempre en el mismo punto
de la mesa, no en la esquina del jugador.

## Cómo se generan

No se editan a mano. Salen del proyecto `tableplace-main`:

```
bun scripts/unmatched/build.ts <set>                 # arte para la web
bun scripts/unmatched/to-unbrewed.ts <set> <héroe>   # escribe aquí <héroe>/ y <set>.json
```
