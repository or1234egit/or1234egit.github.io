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
