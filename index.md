<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css">
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.js"></script>
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/contrib/auto-render.min.js" onload="renderMathInElement(document.body, {delimiters: [{left: '$$', right: '$$', display: true}, {left: '$', right: '$', display: false}, {left: '\\(', right: '\\)', display: false}, {left: '\\[', right: '\\]', display: true}], throwOnError: false});"></script>

# Welcome to My Math Notes

Here you can find my collection of mathematical notes and concepts.

## Test Equations

Here are some inline equations:

- The formula $E = mc^2$ describes mass-energy equivalence
- If $x > 0$, then $\sqrt{x^2} = x$
- The series $\sum_{n=1}^{\infty} \frac{1}{n^2}$ equals $\frac{\pi^2}{6}$

And here are some display equations:

$$ \int_{-\infty}^{\infty} e^{-x^2} \,dx = \sqrt{\pi} $$

<div class="katex-fallback" data-latex="\\int_{-\\infty}^{\\infty} e^{-x^2} \\,dx = \\sqrt{\\pi}"></div>

$$ \frac{d}{dx} e^x = e^x $$

<div class="katex-fallback" data-latex="\\frac{d}{dx} e^x = e^x"></div>

<script>
document.addEventListener('DOMContentLoaded', function(){
  // Render any fallback display math blocks (in case $$...$$ were stripped)
  document.querySelectorAll('.katex-fallback').forEach(function(el){
    var latex = el.getAttribute('data-latex');
    if (latex && window.katex) {
      katex.render(latex, el, {displayMode: true, throwOnError: false});
    }
  });
});
</script>

## Recent Notes

- [Coming soon...]

<!-- Tabs UI for categories -->
<style>
.tabs {display:flex;gap:8px;margin:16px 0}
.tab-btn {padding:8px 12px;border:1px solid #ccc;border-bottom:none;background:#f6f6f6;cursor:pointer}
.tab-btn.active {background:white;border-top:2px solid #0366d6;font-weight:600}
.tab-panels {border:1px solid #ccc;padding:12px;background:white}
.tab-panel {display:none}
.tab-panel.active {display:block}
.summary-link {margin:8px 0}
</style>

<div class="tabs" role="tablist">
  <button class="tab-btn active" data-tab="algebra">Algebra</button>
  <button class="tab-btn" data-tab="calculus">Calculus</button>
</div>
<div class="tab-panels">
  <div id="algebra" class="tab-panel active">
    <h3>Algebra</h3>
    <p>Short notes and links for algebra topics.</p>
    <div class="summary-link">
      <a href="/notes/algebra/linear-algebra.html">Linear Algebra — Vectors and Matrices</a>
      <p class="muted">Dot product, matrices, and examples.</p>
    </div>
  </div>
  <div id="calculus" class="tab-panel">
    <h3>Calculus</h3>
    <p>Short notes and links for calculus topics.</p>
    <div class="summary-link">
      <a href="/notes/calculus/intro-calculus.html">Intro to Calculus — Derivatives</a>
      <p class="muted">Derivatives and rules with examples.</p>
    </div>
  </div>
</div>

<script>
document.querySelectorAll('.tab-btn').forEach(function(btn){
  btn.addEventListener('click', function(){
    document.querySelectorAll('.tab-btn').forEach(b=>b.classList.remove('active'));
    document.querySelectorAll('.tab-panel').forEach(p=>p.classList.remove('active'));
    btn.classList.add('active');
    document.getElementById(btn.dataset.tab).classList.add('active');
  });
});
</script>

<!-- end Tabs UI -->
