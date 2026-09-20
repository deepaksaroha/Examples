# Examples

# Jank

```
<!DOCTYPE html>
<html>
<head>
<style>
.box {
  background: red;
  height: 100px;
  width: 100px;
  animation: moveCPU 2s infinite;
}
@keyframes moveCPU {
  from { margin-left: 200px; }
  to { margin-left: 500px; }
}
</style>

</head>
<body>

<div class="box"></div>
<script>
	setInterval(() => {
		let x=0;
		while(x < 100000000){x = x + 1}
	}, 10)
</script>

</body>
</html>

```


https://github.com/user-attachments/assets/b9b8cfec-6e9d-4bfd-b1a8-29102ddbc69b



