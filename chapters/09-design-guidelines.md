# 9. Design Guidelines & Antipatterns

## Do
- Separate **what/how**: describe workflows with Free syntax; interpret per environment.  
- Make **context a value** (Reader/closures), not globals.  
- **Bracket resources** (withXYZ/bracket) for safety.  
- **Ritualize invariants**: open sessions with shared values; ship tests with specs.  
- Balance archetypes in pods: **Turtle/Wolf/Bear**.

## Don’t
- Couple evaluation to execution (no hard-coded interpreters).  
- Hide invariants (secret policies erode correctness).  
- Over-optimize Wolf (shipping) at Turtle/Bear’s expense.  
- Treat rituals as “soft”—they are the η operation that holds the system together.

---

[← Previous](08-empirical-methods.md) | [Next →](10-ethics-legal.md)
