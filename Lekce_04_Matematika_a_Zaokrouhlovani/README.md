# Efektivní matematika a zaokrouhlování

Jak psát méně kódu při počítání a jak zkrotit dlouhá desetinná čísla.

### 1. Zkrácené zápisy (In-place operátory)
Často potřebujeme změnit hodnotu proměnné (např. přičíst 1 k věku nebo přičíst body v hře). 
Místo dlouhého psaní existuje zkratka:

| Dlouhý zápis | Zkrácený zápis | Co to udělá? |
| :--- | :--- | :--- |
| `x = x + 5` | `x += 5` | Přičte 5 k původní hodnotě |
| `x = x - 2` | `x -= 2` | Odečte 2 |
| `x = x * 3` | `x *= 3` | Vynásobí původní hodnotu |
| `x = x / 4` | `x /= 4` | Vydělí původní hodnotu |

**Pamatuj:** Znaménko je vždy před rovnítkem! `+=`, `-=`, `*=`.

### 2. Zaokrouhlování: `round()`
Python při dělení často vyhazuje čísla jako `3.33333333335`. Pro krásný výstup používáme funkci `round()`.

**Syntaxe:** `round(číslo, počet_míst)`

* `round(3.14159, 2)` -> Výsledek: `3.14`
* `round(3.14159)` -> Výsledek: `3` (zaokrouhlí na celé číslo)

---

## Úkoly v main.py

1. **Zvětšovač:** Uživatel zadá číslo. Pomocí zkráceného zápisu `+=` k němu přičti 10 a výsledek vypiš.
2. **Útrata v hospodě:** Zeptej se na celkovou sumu účtu a počet lidí. Vypiš, kolik má každý zaplatit, ale zaokrouhli to na **2 desetinná místa**.
3. **Plocha kruhu:** Uživatel zadá poloměr `r`. Spočítej plochu ($S = 3.14 * r^2$). Výsledek vypiš zaokrouhlený na **celé číslo**.
