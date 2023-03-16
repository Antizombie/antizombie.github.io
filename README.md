<!DOCTYPE html>
<html>
<head>
	<title>Статическая страница</title>
	<script>
		window.onload = function() {
			var textParam = new URLSearchParams(window.location.search).get('text');
			if (textParam) {
				var textElement = document.getElementById('text');
				textElement.textContent = textParam;
			}
		}
	</script>
</head>
<body>
	<h1>Статическая страница</h1>
	<p>Привет, <span id="text"></span>!</p>
</body>
</html>
