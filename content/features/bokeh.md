

```python
import numpy as np
from bokeh.plotting import figure, show
from bokeh.io import output_notebook

N = 4000
x = np.random.random(size=N) * 100
y = np.random.random(size=N) * 100
radii = np.random.random(size=N) * 1.5
colors = ["#%02d%02d%02d" % (r, g, 150) for r, g in zip(np.floor(50+2*x), np.floor(30+2*y))]
output_notebook()
p = figure()
p.circle(x, y, radius=radii, fill_color=colors, fill_alpha=0.6, line_color=None)
show(p)
```



    <div class="bk-root">
        <a href="https://bokeh.pydata.org" target="_blank" class="bk-logo bk-logo-small bk-logo-notebook"></a>
        <span id="1754">Loading BokehJS ...</span>
    </div>


  <div class="bk-root" id="275ce6f9-3b57-42aa-a155-ab232ffb66e6" data-root-id="1755"></div>




