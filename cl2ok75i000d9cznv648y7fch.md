## GitHub Markdown LaTeX handy tool

There are some ways to write GitHub markdown LaTeX
1. GitHub render server [^1]
  * `<img src="https://render.githubusercontent.com/render/math?math=e^{i \pi} = -1">`
  * `![formula](https://render.githubusercontent.com/render/math?math=e^{i%20\pi}%20=%20-1)`, the space character needs to decode `%20`
  * To change Dark/Light theme
    * Light: `<img src="https://render.githubusercontent.com/render/math?math={e^{i \pi} = -1}#gh-light-mode-only">`
    * Dark: `<img src="https://render.githubusercontent.com/render/math?math={\color{white}e^{i \pi} = -1}#gh-dark-mode-only">`
    * Show: 
<img src="https://render.githubusercontent.com/render/math?math={e^{i \pi} = -1}#gh-light-mode-only">
<img src="https://render.githubusercontent.com/render/math?math={\color{white}e^{i \pi} = -1}#gh-dark-mode-only">

2. Using [readme2tex](https://github.com/leegao/readme2tex), But It's update long time ago
3. Using `mathjax-node` convert to img, need attention using double backslash [^2]

# More examples

<p align="center">
  <a href="#gh-light-mode-only"><img src='https://render.githubusercontent.com/render/math?math=sharks%20=%20\text{%CF%83}_{family%20=%20\text{%22}sharks\text{%22}}(animals)#gh-light-mode-only'></a>
   <a href="#gh-dark-mode-only"><img src='https://render.githubusercontent.com/render/math?math={\color{white}sharks%20=%20\text{%CF%83}_{family%20=%20\text{%22}sharks\text{%22}}(animals)}#gh-dark-mode-only'></a>
</p>

```html
<p align="center">
  <img src='https://render.githubusercontent.com/render/math?math=sharks%20=%20\text{%CF%83}_{family%20=%20\text{%22}sharks\text{%22}}(animals)#gh-light-mode-only'>
  <img src='https://render.githubusercontent.com/render/math?math={\color{white}sharks%20=%20\text{%CF%83}_{family%20=%20\text{%22}sharks\text{%22}}(animals)}#gh-dark-mode-only'>
</p>
```
disable click
```html
<p align="center">
  <a href="#gh-light-mode-only"><img src='https://render.githubusercontent.com/render/math?math=sharks%20=%20\text{%CF%83}_{family%20=%20\text{%22}sharks\text{%22}}(animals)#gh-light-mode-only'></a>
  <a href="#gh-dark-mode-only"><img src='https://render.githubusercontent.com/render/math?math={\color{white}sharks%20=%20\text{%CF%83}_{family%20=%20\text{%22}sharks\text{%22}}(animals)}#gh-dark-mode-only'></a>
</p>
```






[^1]: https://gist.github.com/a-rodin/fef3f543412d6e1ec5b6cf55bf197d7b
[^2]: http://docs.mathjax.org/en/latest/basic/mathematics.html#putting-math-in-javascript-strings