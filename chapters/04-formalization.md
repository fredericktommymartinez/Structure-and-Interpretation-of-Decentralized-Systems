# 4. Formalization

## 4.1 Categorical Model
Let **C** be a category of processes. A monad (T, η, μ) on C yields:
- **η : Id ⇒ T** (pure/return)
- **μ : T² ⇒ T** (flatten/associative composition)

**Interpretation.** `T` wraps contextualized computations. `μ` enforces lawful composition; `η` injects values/rituals.

## 4.2 Interpreters, Effects, and Free Constructions
- Free monads separate **syntax (what)** from **semantics (how)**.
- Effect handlers select operational policies (dev vs. prod; teaching vs. testing; “honor” vs. “risk-on”).

## 4.3 Laws ↔ Failure Modes
| Law | If Violated… | Real-World Symptom |
|---|---|---|
| Left identity | `return a >>= f ≠ f a` | Onboarding rituals don’t “take”; context injection fails |
| Right identity | `m >>= return ≠ m` | Bureaucracy that adds no value |
| Associativity | `(m >>= f) >>= g ≠ m >>= (λa. f a >>= g)` | Coordination chaos; reorgs break outcomes |
| Invariant | Postconditions not preserved | Security/compliance incidents; cultural drift |

---

[← Previous](03-mct.md) | [Next →](05-harmonic-adhocracy.md)
