# web-tabs
a web tabs plugin based on Jquey or Zepto

# demo online
[tabs](http://dannyliou.github.io/demos/tabs/tabs.html)

#USAGE

html
```html
    <div class="tabs">
        <ul class="nav">
            <li name="panel1">TAB1</li>
            <li name="panel2">TAB2</li>
            <li name="panel3">TAB3</li>
            <li name="panel4">TAB4</li>
            <li name="panel5">TAB5</li>
        </ul>
        <div class="panel1">TAB1对应的页面</div>
        <div class="panel2">TAB2对应的页面</div>
        <div class="panel3">TAB3对应的页面</div>
        <div class="panel4">TAB4对应的页面</div>
        <div class="panel5">TAB5对应的页面</div>
    </div>
```
javascript
```javascript
$('.tabs').tabs();
```
