# CSS中的链接样式

- Link (没有访问过的): 这是链接的默认状态，当它没有处在其他状态的时候，它可以使用`:link` 伪类来应用样式。
- Visited: 这个链接已经被访问过了(存在于浏览器的历史纪录), 它可以使用 `:visited` 伪类来应用样式。
- Hover: 当用户的鼠标光标刚好停留在这个链接，它可以使用 `:hover` 伪类来应用样式。
- Focus: 一个链接当它被选中的时候 (比如通过键盘的 Tab  移动到这个链接的时候，或者使用编程的方法来选中这个链接 HTMLElement.focus()) 它可以使用 `:focus` 伪类来应用样式。
- Active: 一个链接当它被激活的时候 (比如被点击的时候)，它可以使用 `:active` 伪类来应用样式。


这里有一些属性可以更改样式（不仅限于这些）：

- color 文字的颜色
- cursor 鼠标光标的样式，你不应该把这个关掉，除非你有非常好的理由。
- outline 文字的轮廓 (轮廓有点像边框，唯一的区别是边框占用了盒模型的空间，而轮廓没有； 它只是设置在背景图片的顶部)。outline 有一个有用的辅助功能，所以在把它关掉之前考虑清楚；你应该至少将 选中 (focus) 状态上链接悬停 (hover) 状态的样式加倍。