# web-tabs
a web tabs plugin based on jQuey or Zepto

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
//init
$('.tabs').tabs({
    navSelector: '.nav li',//nav btn selector
    showName: null,//the default showing panel class name
    activeClass: 'active',//selected nav btn classname
    menuAttr: 'name'//nav btn's attribute to link the showing panel
});
```

#API & EVENT

## ATTENTION
the following api and event functions must be called after init 

javascript
```javascript
    //api
    var tabsInstance = $('.tabs').getTabs();
    tabsInstance.show('panel3');
    
    //event
    $('.tabs').on('tabs:show', function(ev, prename, curname) {
        console.log(prename, curname);
    })
    $('.tabs').on('tabs:hide', function(ev, name) {
        console.log(name);
    })
```
