# xveco

Librería de economía simulada en Python.

## 💰 Características

- Cuentas con dinero en céntimos
- Transferencias entre usuarios
- Sistema de inflación
- Banco con dinero limitado
- Préstamos con interés
- Sistema de deuda

---

## 🚀 Ejemplo básico

```python
import xveco

coin = xveco.Currency("XCoin", "X", 0.5, "🪙")

santi = xveco.Account("Santi", coin)
pepe = xveco.Account("Pepe", coin)

santi.deposit(100)
pepe.deposit(50)

santi.transfer(pepe, 25)

coin.apply_inflation(10)