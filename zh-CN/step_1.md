要使用 CSS 显示或隐藏 HTML 元素，可以使用 display 属性。 你可以使用不同的 display 属性值：

- 在你的 CSS 样式表中，您可以使用 `display: none;`。 该值将元素完全隐藏，并且不会占用页面上的任何空间。

## --- code ---

language: css
filename:
line_numbers: true
-------------------------------------------------------

.hide {
display: none;
}

\--- /code ---

然后，在你的 HTML 文件中，你可以将该类应用于你想要隐藏的元素。

## --- code ---

language: html
filename:
line_numbers: true
-------------------------------------------------------

```
<div class="hide">此元素已隐藏。</div>
```

\--- /code ---

- 要显示元素，你还可以在 CSS 样式表中创建选择器并使用属性 `display: block;`。

## --- code ---

language: css
filename:
line_numbers: true
-------------------------------------------------------

.hide {
display: none;
}

.show {
display: block; /\* or inline, inline-block, etc. \*/
}

\--- /code ---

## --- code ---

language: html
filename:
line_numbers: true
-------------------------------------------------------

```
<div class="hide">此元素最初是隐藏的。</div>
<div class="show">此元素最初是可见的。</div>
```

\--- /code ---

- 你还可以使用 JavaScript 来切换 HTML 元素的可见性。 这将使它出现和消失。

## --- code ---

language: js
filename:
line_numbers: true
-------------------------------------------------------

var element = document.querySelector(#myElement);

// 隐藏元素
element.style.display = "none";

// 显示元素
element.style.display = "block";

\--- /code ---
