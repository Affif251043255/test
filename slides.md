---
title-slide: false
bibliography: references.bib
csl: vancouver.csl
citeproc: true
theme: serif
background-color: "#ffffff"
transition: slide
navigationMode: linear
hash: true
---

:::: {.columns}
::: {.column width="50%"}

## Sample slides
#### PlaceHolderName
#### Universiti Malaysia Perlis
#### [placeholder@email.com](mailto:placeholder@email.com)

<audio id="bg-music" src="media/audio/sb.m4a" loop></audio>

<div id="audio-credit"
     style="position: absolute; bottom: 40px; right: 20px; font-size: 0.6em; opacity: 0.6;">
  Music: “Adrift” by Scott Buckley (CC BY 4.0)
</div>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    const audio = document.getElementById('bg-music');
    const credit = document.getElementById('audio-credit');

    // hide credit by default
    credit.style.display = 'none';

    const test = new Audio('media/audio/bgm.mp3');

    test.addEventListener('canplaythrough', () => {
      // bgm.mp3 exists → use it, keep credit hidden
      audio.src = 'media/audio/bgm.mp3';
    }, { once: true });

    test.addEventListener('error', () => {
      // bgm.mp3 missing → sb.m4a will play → show credit
      credit.style.display = 'block';
    }, { once: true });

    document.addEventListener('click', () => {
      if (Reveal.getIndices().h === 0) {
        audio.volume = 0.5;
        audio.play();
      }
    }, { once: true });

    Reveal.on('slidechanged', (event) => {
      if (event.indexh > 0) { audio.pause(); }
      else { audio.play(); }
    });
  });
</script>

:::

::: {.column width="50%"}
![](media/pics/logo1.png)
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide one
**Key Concepts:**
- Energy conservation per @carnot1824.
- $\Delta U = Q - W$
:::

::: {.column width="50%"}
![](media/pics/sample.png)
:::
::::

---

<span class="slide-title" data-title="My Hidden Slide Name"></span>

![](media/pics/wide.jpeg)

---

:::: {.columns}
::: {.column width="50%"}
### The Master Equation
The fundamental relation of thermodynamics:

$$\Delta U = Q - W$$

The work done $W$ is positive when the system expands against an external pressure.
:::

::: {.column width="50%"}
<video data-src="media/videos/sample.mp4" data-autoplay loop muted width="100%"></video>
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Visualizing the Gas Law
**Interactive Model:**

- P, V, and T relationships.
- Use the slider to adjust pressure.
- Observe the phase boundary.
:::

::: {.column width="50%"}
<iframe 
  data-src="media/plots/sample.html" 
  width="100%" 
  height="500px" 
  style="border:none;" 
  scrolling="no">
</iframe>
:::
::::

---

# Bibliography
<div id="refs"></div>

---

:::: {.columns}
::: {.column width="50%"}
### Part Length Distribution

This histogram visualizes the distribution of 'Part Length' from the 'X002' dataset, showing the frequency of different part length values.
:::

::: {.column width="50%"}
<iframe 
  data-src='media/plots/x002_partlength_histogram.html' 
  width='100%' 
  height='500px' 
  style='border:none;' 
  scrolling='no'>
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Part Length Box Plot

This box plot displays the distribution of 'Part Length' from the 'X002' dataset, showing its median, quartiles, and potential outliers.
:::

::: {.column width="50%"}
<iframe 
  data-src='media/plots/x002_partlength_boxplot.html' 
  width='100%' 
  height='500px' 
  style='border:none;' 
  scrolling='no'>
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Part Length vs Part Resistance

This scatter plot illustrates the relationship between 'Part Length' and 'Part Resistance' from the 'X002' dataset, helping to identify potential correlations or patterns between these two process parameters.
:::

::: {.column width="50%"}
<iframe 
  data-src='media/plots/x002_partlength_partresistance_scatter.html' 
  width='100%' 
  height='500px' 
  style='border:none;' 
  scrolling='no'>
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Average Part Length by Machine

This bar chart illustrates the average 'Part Length' for each 'Machine' from the 'X002' dataset, allowing for easy comparison of part length performance across different machines.
:::

::: {.column width="50%"}
<iframe 
  data-src='media/plots/x002_avg_partlength_barchart.html' 
  width='100%' 
  height='500px' 
  style='border:none;' 
  scrolling='no'>
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Analysis
**Parameters:**
- Pressure: 200kPa
- Temperature: 338K
- Target: 50 $\pm$ 5

This control chart monitors the process stability for Machine 1.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Capability

Visualizing the distribution of Part Length against the Lower Specification Limit (45) and Upper Specification Limit (55).
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_capability.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Analysis
Control chart monitoring for Machine 2 under identical settings.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Capability
Process capability histogram for Machine 2.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_capability.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Analysis
Control chart monitoring for Machine 3.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Capability
Process capability histogram for Machine 3.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_capability.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Control Chart
Individual measurements (X) for Machine 1.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Moving Range
Moving Range (MR) chart for Machine 1, tracking the absolute difference between consecutive points.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_m_chart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Control Chart
Individual measurements (X) for Machine 2.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Moving Range
Moving Range (MR) chart for Machine 2.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_m_chart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Control Chart
Individual measurements (X) for Machine 3.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Moving Range
Moving Range (MR) chart for Machine 3.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_m_chart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Analysis
- **Type:** Individuals Chart
- **Parameter:** Part Length

Monitoring individual measurements to detect shifts in the process mean.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Variation
- **Type:** Moving Range (MR) Chart
- **Parameter:** Range between parts

Monitoring short-term variability to ensure consistent performance.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_m_chart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Analysis
Individuals Control Chart for Machine 2 measurements.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Variation
Moving Range (MR) chart for Machine 2 variability.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_m_chart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Analysis
Individuals Control Chart for Machine 3 measurements.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Variation
Moving Range (MR) chart for Machine 3 variability.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_m_chart.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Control Chart
Individual measurements (X) for Machine 1.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Capability Analysis
Full statistical analysis ($C_p, C_{pk}$) for Machine 1 showing how well the process stays within the limits ($LSL=45, USL=55$).
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_capability.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Control Chart
Individual measurements (X) for Machine 2.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Capability Analysis
Full statistical analysis for Machine 2.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_capability.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Control Chart
Individual measurements (X) for Machine 3.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Capability Analysis
Full statistical analysis for Machine 3.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_capability.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::
