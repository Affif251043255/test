---
title-slide: false
theme: serif
---

# Machine Performance Report

---

## Machine 1: Stability

:::: {.columns}
::: {.column width="50%"}
### I-Chart Analysis
Machine 1 operates within control limits with no violations in the first 200 samples.

**Status:** Unstable
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_ichart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

## Machine 1: Capability

:::: {.columns}
::: {.column width="50%"}
### Capability Indices
- $C_p$: 1.524
- $C_{pk}$: 1.429
- $C_{pm}$: 1.465
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_cap.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

## Machine 2: Stability

:::: {.columns}
::: {.column width="50%"}
### I-Chart Analysis
Monitoring Machine 2 stability.

**Status:** Stable
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_ichart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

## Machine 2: Capability

:::: {.columns}
::: {.column width="50%"}
### Capability Indices
- $C_p$: 2.828
- $C_{pk}$: 2.818
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_cap.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

## Machine 3: Stability

:::: {.columns}
::: {.column width="50%"}
### I-Chart Analysis
Monitoring Machine 3 stability.

**Status:** Stable
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_ichart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

## Machine 3: Capability

:::: {.columns}
::: {.column width="50%"}
### Capability Indices
- $C_p$: 1.372
- $C_{pk}$: 1.073
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_cap.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

## Performance Comparison

### Ranking Summary
|   Machine | Stability   |    Cp |   Cpk |   Cpl |   Cpu |   Cpm |   Rank |
|----------:|:------------|------:|------:|------:|------:|------:|-------:|
|         2 | Stable      | 2.828 | 2.818 | 2.837 | 2.818 | 2.826 |      1 |
|         1 | Unstable    | 1.524 | 1.429 | 1.429 | 1.619 | 1.465 |      2 |
|         3 | Stable      | 1.372 | 1.073 | 1.671 | 1.073 | 1.021 |      3 |

**Conclusion:** Machine 2 is the top performer.
