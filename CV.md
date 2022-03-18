---
layout: default
---
# CV 
---
<iframe src="assets/Razik_CV.pdf" id="Razik_CV-iframe"></iframe>

<script>
	let iframe = document.querySelector("#child-iframe");

	iframe.addEventListener('load', function() {
		iframe.style.height = iframe.contentDocument.body.scrollHeight + 'px';
		iframe.style.width = iframe.contentDocument.body.scrollWidth + 'px';
	});	
</script>
