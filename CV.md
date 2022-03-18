---
layout: default
---
# CV 
---
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>JavaScript Auto Adjust iFrame Height Based on Content</title>
<style>
    iframe{
        width: 100%;
        border: 2px solid #ccc;
    }
</style>
</head>
<body>
    <iframe src="assets/Razik_CV.pdf" id="myIframe"></iframe>
    
    <script>
    // Selecting the iframe element
    var iframe = document.getElementById("myIframe");
    
    // Adjusting the iframe height onload event
    iframe.onload = function(){
        iframe.style.height = iframe.contentWindow.document.body.scrollHeight + 'px';
    }
    </script>
</body>
</html>
