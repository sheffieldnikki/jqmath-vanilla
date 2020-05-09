# jqmath-vanilla
Pure JavaScript version of jqMath math rendering library, so doesn't require jQuery. 
Forked from jqMath v0.4.6 (May-2016) which is copyright 2016, Mathscribe, Inc. and released under the MIT license.

jqMath makes it easy to put formatted mathematical expressions in web pages. 
Use a simple TeX-like syntax to write expressions directly into your HTML.

If \$ax^2+bx+c=0\$ with \$aâ‰ 0\$, then: \$\$x={-bÂ±âˆš{b^2-4ac}}/{2a}\$\$

<table border='1'>
<thead><tr><th>Math Library</th><th>Release</th><th>Example page</th><th>HTTP<br/>requests</th><th>Transfer<br/>kB</th><th>First<br/>load</th><th>Cached<br/>load</th><th>Browser support</th></tr></thead>
<tbody>
<tr><td><b>Vanilla jqMath</b></td><td><i>n/a</i><br/>May-2020</td><td>[<a href='jqmath-vanilla.html'>example page</a>]</td>
    <td class='good'>3</td><td class='good'>&nbsp;18.3</td><td class='good'>0.54s</td><td class='good'>0.47s</td><td>IE9+, Edge, FF?, Chrome ?, Safari ?, Opera ?</td></tr>
<tr><td><b><a href='https://mathscribe.com/author/jqmath.html' target='_blank' title='jqMath homepage'>jqMath with jQuery</a></b></td><td>v0.4.6<br/>May-2016</td><td>[<a href='jqmath-jquery.html'>example page</a>]</td>
    <td>8</td><td>&nbsp;81.9</td><td>1.03s</td><td>0.90s</td><td>IE6+, FF2+, Chrome, Safari 3+, Opera 9+</td></tr>
<tr><td><b><a href='https://katex.org/' target='_blank' title='KaTeX homepage'>KaTeX</a></b><sup>1</sup></td><td>v0.11.1<br/>Sep-2019</td><td>[<a href='katex.html'>example page</a>]</td>
    <td class='bad'>14</td><td class='bad'>215.7</td><td>1.67s</td><td>1.19s</td><td>IE9+, Edge, FF?, Chrome ?, Safari ?, Opera ?</td></tr>
<tr><td><b><a href='https://www.mathjax.org/' target='_blank' title='MathJax homepage'>MathJax with polyfill</a></b><sup>2</sup></td><td>v3.0.5<br/>Mar-2020</td><td>[<a href='mathjax.html'>example page</a>]</td>
    <td class='bad'>15</td><td class='bad'>291.6</td><td class='bad'>3.67s</td><td class='bad'>2.66s</td><td>IE11+, Edge, FF38+, Chrome 29+, Safari 9+, Opera 33+, iOS 9+, Android 4+</td></tr>
</tbody>
</table>
