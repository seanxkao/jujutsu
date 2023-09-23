<!DOCTYPE html>
<html>
	<head>
		<title>五條體生成器</title>
	</head>

	<body>
		<h1>五條體生成器</h1>
		<div>
			<input id="character" placeholder="宿儺"> 真是太強了
		</div>
		<div>
			就算沒有 <input id="object" placeholder="十影"></input> 也會贏
		</div>
		<div>
			殺死我的不是 <input id="thing1" placeholder="時間"></input> 或 <input id="thing2" placeholder="疾病"></input>
		</div>
		<button type="button" id="mainButton">真是太好了</button>
		<div>
			<textarea id="output" style="width:400px;height:200px;"></textarea>
		</div>
	</body>

	<script>
		var button = document.getElementById("mainButton")
		var characterInput = document.getElementById("character")
		var objectInput = document.getElementById("object")
		var thing1Input = document.getElementById("thing1")
		var thing2Input = document.getElementById("thing2")
		var output = document.getElementById("output")
		button.onclick = function()
		{
			var result = [];
			result.push(
			  characterInput.value + "太強了",
			  "而且" + characterInput.value + "還沒有使出全力的樣子",
			  "對方就算沒有" + objectInput.value + "也會贏",
			  "我甚至覺得有點對不起他",
			  "我沒能在這場戰鬥讓" + characterInput.value + "展現他的全部給我",
			  "殺死我的不是" + thing1Input.value + "或" + thing2Input.value,
			  "而是比我更強的傢伙，真是太好了",
			);
			output.value = result.join("\n");
		};
	</script>

</html>
