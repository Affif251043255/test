---
title: Manufacturing Quality Report
theme: serif
---

# SPC & Capability Analysis

---

## Global Comparison Table

|   Machine |   Mean |   StdDev | Stability     |    Cp |   Cpk |   Cpm | Capable   |   Rank |
|----------:|-------:|---------:|:--------------|------:|------:|------:|:----------|-------:|
|         2 | 49.985 |    0.548 | Special Cause | 3.06  | 3.051 | 3.059 | Yes       |      1 |
|         1 | 49.661 |    1.141 | Special Cause | 1.474 | 1.374 | 1.412 | Yes       |      2 |
|         3 | 51.172 |    1.185 | Special Cause | 1.387 | 1.062 | 0.993 | No        |      3 |

**Best Performer:** Machine 2

---

## Machine 2: SPC & Capability

:::: {.columns}
::: {.column width="50%"}
### Statistical Summary
- **Stability:** Special Cause
- **Mean:** 49.985 mm
- **Cpk:** 3.051
- **Capable (1.33):** Yes

*Target: 50.0 | Tolerance: ±5.0*
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_cap.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

## Machine 1: SPC & Capability

:::: {.columns}
::: {.column width="50%"}
### Statistical Summary
- **Stability:** Special Cause
- **Mean:** 49.661 mm
- **Cpk:** 1.374
- **Capable (1.33):** Yes

*Target: 50.0 | Tolerance: ±5.0*
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_cap.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

## Machine 3: SPC & Capability

:::: {.columns}
::: {.column width="50%"}
### Statistical Summary
- **Stability:** Special Cause
- **Mean:** 51.172 mm
- **Cpk:** 1.062
- **Capable (1.33):** No

*Target: 50.0 | Tolerance: ±5.0*
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_cap.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::
