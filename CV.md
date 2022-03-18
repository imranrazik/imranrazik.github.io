---
layout: default
---
# CV 
---

function resizer(id)
{

var doc=document.getElementById(id).contentWindow.document;
var body_ = doc.body, html_ = doc.documentElement;

var height = Math.max( body_.scrollHeight, body_.offsetHeight, html_.clientHeight, html_.scrollHeight, html_.offsetHeight );
var width  = Math.max( body_.scrollWidth, body_.offsetWidth, html_.clientWidth, html_.scrollWidth, html_.offsetWidth );

document.getElementById(id).style.height=height;
document.getElementById(id).style.width=width;

}

<IFRAME SRC="https://docs.google.com/viewer?srcid=1jwOZwp416fbD2iPgwD4ufFyyjjgGmNsH&pid=explorer&efh=false&a=v&chrome=false&embedded=true" id="iframe1"  onLoad="resizer('iframe1');"></iframe>
