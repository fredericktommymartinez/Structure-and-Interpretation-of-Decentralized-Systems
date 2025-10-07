# 7. Case Studies

## 7.1 BTCU: Education as a Monadic Pipeline
- **Atomic:** handle failure (wallet setup, gas, BNS) via Either  
- **Domain:** pass env (Reader Config)  
- **Control:** resource safety (credential issuance, payouts)  
- **Orchestration:** Free/effects to swap “X Spaces”, “Discord”, “YouTube” handlers  
**Outcomes:** completion rate, time-to-wallet, support load, educator payout latency.

## 7.2 Stacks AI Guild: Apprenticeship as Effect Stacks
- Apprentices’ work = `Reader(env) ∘ State(repo) ∘ Writer(docs) ∘ IO(ci)`  
- AI suggests pairings; detects imbalance (“too much Wolf, add Turtle sprint”)

## 7.3 Dojo Logic OS: Formal Combat Interpreter
- **Syntax:** predicates (isReversalMove, isAntiAir)  
- **Evaluator:** rule engine + temporal belief store  
- **Handlers:** “Training”, “Tournament”, “Honor” policies  
- **Properties:** reversal soundness; combo associativity; Denjin monotonicity

## 7.4 Tokenized Travel: Liquidity & Governance Hooks
- Credits token with hooks: treasury split, loyalty rebates, anti-abuse windows  
- DAO orchestrates resort onboarding policies via Free semantics

---

[← Previous](06-ai-coordination.md) | [Next →](08-empirical-methods.md)
