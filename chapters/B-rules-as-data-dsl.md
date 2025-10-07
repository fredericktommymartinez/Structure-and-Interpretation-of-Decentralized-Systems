# Appendix B — Rules-as-Data DSL (snippet)

```yaml
rule: antiAir
if:
  - pred: hitboxHeight
    op: '>'
    args: [m, characterHeight]
  - pred: upperBodyInvuln
    args: [m]
  - pred: leq
    args: [startupFrames(m), 7]
then:
  - pred: tag
    args: [m, "anti_air"]


### `appendices/C-property-tests.md`
```markdown
# Appendix C — Property Tests (examples)

- **Associativity (combos):**  
  `valid(a,b) ∧ valid(b,c) ⇒ valid(a, b∘c)` (under pushback/range composition)

- **Resource safety:**  
  `withFile(f)(use) ⇒ fileClosed(f)` even under exceptions

- **Incentive fairness:**  
  Rotation preserves median wait time per archetype within ε
