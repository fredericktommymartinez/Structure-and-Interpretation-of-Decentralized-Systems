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
