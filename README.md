<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HyperLock</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial, sans-serif;
}

body{
background:#0f0f0f;
color:white;
display:flex;
justify-content:center;
align-items:center;
min-height:100vh;
}

.card{
width:350px;
background:#1b1b1b;
border-radius:20px;
padding:25px;
box-shadow:0 0 20px rgba(255,0,0,.2);
}

.logo{
text-align:center;
font-size:32px;
font-weight:bold;
color:#ff3b3b;
margin-bottom:5px;
}

.author{
text-align:center;
opacity:.8;
margin-bottom:25px;
}

.item{
display:flex;
justify-content:space-between;
align-items:center;
padding:12px 0;
border-bottom:1px solid #333;
}

.switch{
width:50px;
height:26px;
background:#444;
border-radius:30px;
position:relative;
cursor:pointer;
}

.switch::before{
content:"";
position:absolute;
width:20px;
height:20px;
left:3px;
top:3px;
background:white;
border-radius:50%;
transition:.3s;
}

.switch.active{
background:#ff0000;
}

.switch.active::before{
transform:translateX(24px);
}

.btn{
margin-top:20px;
width:100%;
padding:12px;
background:#ff0000;
border:none;
border-radius:10px;
color:white;
font-weight:bold;
cursor:pointer;
}

.info{
margin-top:20px;
font-size:13px;
opacity:.8;
text-align:center;
}
</style>
</head>

<body>

<div class="card">

<div class="logo">HYPERLOCK</div>
<div class="author">By Duc Bao</div>

<div class="item">
<span>Nhẹ Tâm 👾</span>
<div class="switch active"></div>
</div>

<div class="item">
<span>Boost FPS😈</span>
<div class="switch"></div>
</div>

<div class="item">
<span>Nhạy Màn🫀</span>
<div class="switch active"></div>
</div>

<div class="item">
<span>Aimlock👙</span>
<div class="switch"></div>
</div>

<button class="btn">Chạy File</button>

<div class="info">
Developer: Duc Bao<br>
Version 1.0
</div>

</div>

<script>
document.querySelectorAll(".switch").forEach(sw=>{
sw.onclick=()=>{
sw.classList.toggle("active");
}
})
</script>

</body>
</html>