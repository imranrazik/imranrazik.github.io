---
layout: default
---
# CV 
---
<script type="application/javascript">

function resizeIFrameToFitContent( iFrame ) {

    iFrame.width  = iFrame.contentWindow.document.body.scrollWidth;
    iFrame.height = iFrame.contentWindow.document.body.scrollHeight;
}

window.addEventListener('DOMContentLoaded', function(e) {

    var iFrame = document.getElementById( 'iFrame1' );
    resizeIFrameToFitContent( iFrame );

    // or, to resize all iframes:
    var iframes = document.querySelectorAll("iframe");
    for( var i = 0; i < iframes.length; i++) {
        resizeIFrameToFitContent( iframes[i] );
    }
} );

</script>

<iframe src="https://docs.google.com/viewer?srcid=1jwOZwp416fbD2iPgwD4ufFyyjjgGmNsH&pid=explorer&efh=false&a=v&chrome=false&embedded=true" id="iFrame1"></iframe>

