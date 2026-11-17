<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Round Off Calculator</title>
<style>
body{font-family:Arial;background:#f0f0f0;text-align:center;padding:20px}
.box{background:white;max-width:400px;margin:auto;padding:20px;border-radius:10px}
input{width:90%;padding:12px;font-size:18px;margin:10px}
button{width:95%;padding:12px;background:#4CAF50;color:white;border:none;font-size:18px;border-radius:5px}
#result{font-size:24px;font-weight:bold;margin-top:15px;color:#333}
</style>
</head>
<body>
<h1>Round Off Calculator</h1>
<div class="box">
<h3>Enter Your Number</h3>
<input type="number" id="num" placeholder="e.g. 12.6">
<br>
<button onclick="calc()">Calculate</button>
<div id="result"></div>
</div>
<script>
function calc(){
let n = parseFloat(document.getElementById("num").value);
if(isNaN(n)){document.getElementById("result").innerHTML="Please enter a number";return;}
document.getElementById("result").innerHTML="Round Off = " + Math.round(n);
}
</script>
</body>
</html>
