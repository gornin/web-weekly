为不同层级的标签添加背景色

```javascript
// create a bookmark and use this code as the URL, you can now toggle the css on/off
// thanks+credit: https://dev.to/gajus/my-favorite-css-hack-32g3
javascript: (function() {
	var elements = document.body.getElementsByTagName('*');
	var items = [];
	for (var i = 0; i < elements.length; i++) {
		if (elements[i].innerHTML.indexOf('* { background:#000!important;color:#0f0!important;outline:solid #f00 1px!important; background-color: rgba(255,0,0,.2) !important; }') != -1) {
			items.push(elements[i]);
		}
	}
	if (items.length > 0) {
		for (var i = 0; i < items.length; i++) {
			items[i].innerHTML = '';
		}
	} else {
		document.body.innerHTML +=
			'<style>* { background:#000!important;color:#0f0!important;outline:solid #f00 1px!important; background-color: rgba(255,0,0,.2) !important; }\
            * * { background-color: rgba(0,255,0,.2) !important; }\
            * * * { background-color: rgba(0,0,255,.2) !important; }\
            * * * * { background-color: rgba(255,0,255,.2) !important; }\
            * * * * * { background-color: rgba(0,255,255,.2) !important; }\
            * * * * * * { background-color: rgba(255,255,0,.2) !important; }\
            * * * * * * * { background-color: rgba(255,0,0,.2) !important; }\
            * * * * * * * * { background-color: rgba(0,255,0,.2) !important; }\
            * * * * * * * * * { background-color: rgba(0,0,255,.2) !important; }</style>';
	}
})();

// ---------------------------------------------------------
// another bookmarklet to display the elements Id on screen, some of them do display themselves on top of others

javascript: (function () {
  var styleEl = document.getElementById("css-id-labels-hack");
  if (styleEl) {
    styleEl.remove();
    const elems = document.querySelectorAll(".css-idlabel-dbg");
    [...elems].forEach((elem) => {
      elem.remove();
    });
    return;
  }

  styleEl = document.createElement("style");
  styleEl.id = "css-id-labels-hack";
  styleEl.innerHTML =
    "div.css-idlabel-dbg{   text-shadow: 3px 3px 4px white; position: fixed;    background-color: rgba(0,255,0,0.4) !important;    outline: 0px !important;    color: rgb(0, 0, 0) !important;    padding: 2px !important;} ";
  document.body.append(styleEl);
  
  const elems = document.querySelectorAll("[id]");
  [...elems].forEach((elem) => {
    const divroot = document.createElement("div");
    divroot.setAttribute("class", "css-idlabel-dbg");
    divroot.textContent = "#" + elem.id;
    elem.insertAdjacentElement("afterbegin", divroot);
  });

})();
```