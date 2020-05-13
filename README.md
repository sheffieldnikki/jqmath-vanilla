# jQmath-vanilla
Pure JavaScript version of jqMath math rendering library, so doesn't require jQuery. 
Forked from jqMath v0.4.6 (May-2016) which is copyright 2016, Mathscribe, Inc. and released under the MIT license.

jqMath makes it easy to put formatted mathematical expressions in web pages. 
Use a simple TeX-like syntax to write expressions directly into your HTML. e.g.,

`If $ax^2+bx+c=0$ with $a≠0$, then: $$x={-b±√{b^2-4ac}}/{2a}$$`

produces the following:

![Example expression](examples/example.png)

jqMath-vanilla is very lightweight (38.6kB total, or 14.7kB Brotli compressed), fast and concise. It is standards-based and cross-browser, using MathML when available, else simple HTML and CSS, and avoiding pixel-map images. Thus pages load quickly, and expressions can be resized by the user, or easily passed to screen reading, graphing, or computer algebra software.

<h2>Using the library</h2>

Copy the CSS & JS files to your server, and include them in the `<head>` section of your page:
    
    <!DOCTYPE html>
    <html lang="en" xmlns:m="http://www.w3.org/1998/Math/MathML">
    <head>
    <meta charset="utf-8">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=UnifrakturMaguntia">
    <link rel="stylesheet" href="jqmath-0.4.3.min.css">
    <script src="jqmath-vanilla.min.js"></script>
    ...
    </head>

The font stylesheet is only needed if you are using Fraktur letters in your maths.

See the <a href='https://sheffieldnick.github.io/jqmath-vanilla/examples/jqmath-vanilla.html'>example page</a> for an overview, and full documentation is on the original <a href='https://mathscribe.com/author/jqmath.html' target='_blank'>jqMath homepage</a>.

<h2>Math rendering libraries</h2>

<table border='1'>
<thead><tr><th>Math Library</th><th>Release</th><th>HTTP<br/>requests</th><th>Transfer<br/>kB</th><th>First<br/>load</th><th>Cached<br/>load</th><th>Browser support</th></tr></thead>
<tbody>
<tr><td><b>jqMath vanilla</b><br/>[<a href='https://sheffieldnick.github.io/jqmath-vanilla/examples/jqmath-vanilla.html'>example page</a>]</td><td>v0.1.0<br/>May-2020</td>
    <td>3</td><td>&nbsp;18.2</td><td>0.54s</td><td>0.47s</td><td>IE6+, Edge, FF3.5+, Chrome 14+, Safari 3.1+, Opera 9+</td></tr>
<tr><td><b><a href='https://mathscribe.com/author/jqmath.html' target='_blank' title='jqMath homepage'>jqMath+jQuery</a></b><br/>[<a href='https://sheffieldnick.github.io/jqmath-vanilla/examples/jqmath-jquery.html'>example page</a>]</td><td>v0.4.6<br/>May-2016</td>
    <td>8</td><td>&nbsp;81.9</td><td>1.03s</td><td>0.90s</td><td>IE6+, Edge, FF2+, Chrome 16+, Safari 3+, Opera 9+</td></tr>
<tr><td><b><a href='https://katex.org/' target='_blank' title='KaTeX homepage'>KaTeX</a></b><sup>1</sup><br/>[<a href='https://sheffieldnick.github.io/jqmath-vanilla/examples/katex.html'>example page</a>]</td><td>v0.11.1<br/>Sep-2019</td>
    <td>14</td><td>215.7</td><td>1.67s</td><td>1.19s</td><td>IE9+, Edge, FF?, Chrome ?, Safari ?, Opera ?</td></tr>
<tr><td><b><a href='https://www.mathjax.org/' target='_blank' title='MathJax homepage'>MathJax+polyfill</a></b><sup>2</sup><br/>[<a href='https://sheffieldnick.github.io/jqmath-vanilla/examples/mathjax.html'>example page</a>]</td><td>v3.0.5<br/>Mar-2020</td>
    <td>15</td><td>291.6</td><td>3.67s</td><td>2.66s</td><td>IE11+, Edge, FF38+, Chrome 29+, Safari 9+, Opera 33+, iOS 9+, Android 4+</td></tr>
</tbody>
</table>
The download transfer size &amp; load <i>time-until-idle</i> of each page in <code>/examples/</code> was performed with FF76 on a desktop PC.<br/>
<sup>1</sup>KaTeX can alternatively be run server-side for compatibility with <u>all</u> browsers<br/>
<sup>2</sup>MathJax v2.x supports older browsers including IE6-10
