# 3. Monadic Coordination Theory (MCT)

## 3.1 Constraints of Composition
To compose safely under uncertainty and change, a system requires:
- **Associativity**: (a ⋄ b) ⋄ c ≡ a ⋄ (b ⋄ c)
- **Identity**: neutral injection of context/value
- **Invariant preservation**: local steps must not violate global rules

## 3.2 The Four Layers
- **Atomic —** uncertainty & error  
  *Patterns:* Option/Maybe, Either/Result, Validation  
  *Social analog:* ritual repair, forgiveness, graceful failure
- **Domain —** context & state  
  *Patterns:* Reader, State, Writer  
  *Social analog:* lineage, roles, documentation, metrics
- **Control —** boundaries & resources  
  *Patterns:* IO, Resource/bracket, STM  
  *Social analog:* councils, charters, budgets, conflict mediation
- **Orchestration —** heterogeneity & policy  
  *Patterns:* Free, effect systems, transformers  
  *Social analog:* constitutional law, DAO governance, metarules

## 3.3 The Inevitability Thesis
**Theorem (informal).** Any coordination mechanism satisfying the above constraints admits a monadic presentation up to isomorphism of behaviors.  
**Intuition.** If you need a unit (`return`) and a composition (`bind`) that respects invariants and grouping, you have, in essence, a monad.

---

[← Previous](02-background.md) | [Next →](04-formalization.md)
