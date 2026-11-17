# Unbrewed heroes

Mazos de Unmatched (Restoration Games) en el formato nativo de [Unbrewed](https://unbrewed.xyz),
para partidas privadas. El arte es de Restoration Games.

## Importar un mazo en Unbrewed

En **unbrewed.xyz/bag**, pega el enlace al JSON del héroe en la barra de añadir:

| Héroe | Enlace |
|---|---|
| Sherlock Holmes | `https://raw.githubusercontent.com/alexkhudov2002/Unmatched/main/sherlock-holmes/sherlock-holmes.json` |

## Cómo se generan

No se editan a mano. Salen del proyecto `tableplace-main`:

```
bun scripts/unmatched/build.ts <set>                 # arte para la web
bun scripts/unmatched/to-unbrewed.ts <set> <héroe>   # escribe aquí <héroe>/
```
