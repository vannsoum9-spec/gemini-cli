<!DOCTYPE html>
<html lang="km">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>សារណាបញ្ចប់ការសិក្សា - UI</title>

<link href="https://fonts.googleapis.com/css2?family=Khmer+OS+Battambang&family=Khmer+OS+Muol+Light&display=swap" rel="stylesheet">

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>

:root{
--primary:#003366;
--secondary:#cc0000;
--gold:#d4af37;
--bg:#f4f6f8;
}

*{
box-sizing:border-box;
margin:0;
padding:0;
}

body{
font-family:'Khmer OS Battambang',sans-serif;
background:var(--bg);
color:#333;
scroll-behavior:smooth;
}

/* Sidebar */

.sidebar{
position:fixed;
left:0;
top:0;
width:260px;
height:100vh;
background:var(--primary);
color:white;
padding:20px;
overflow:auto;
}

.sidebar h2{
font-family:'Khmer OS Muol Light';
font-size:15px;
text-align:center;
margin-bottom:20px;
}

.sidebar a{
display:block;
padding:12px;
color:white;
text-decoration:none;
font-size:14px;
border-bottom:1px solid rgba(255,255,255,0.1);
}

.sidebar a:hover{
background:var(--secondary);
padding-left:18px;
transition:.3s;
}

/* Content */

.main{
margin-left:260px;
padding:40px;
}

.section{
background:white;
padding:60px;
margin-bottom:40px;
box-shadow:0 0 15px rgba(0,0,0,0.1);
}

.title{
font-family:'Khmer OS Muol Light';
font-size:22px;
color:var(--primary);
margin-bottom:20px;
border-left:6px solid var(--secondary);
padding-left:12px;
}

/* Table */

table{
width:100%;
border-collapse:collapse;
margin-top:20px;
}

th{
background:var(--primary);
color:white;
padding:12px;
}

td{
border:1px solid #ddd;
padding:10px;
}

tr:nth-child(even){
background:#f2f2f2;
}

/* Charts */

.chart-box{
max-width:600px;
margin:auto;
}

/* Back to top */

.top-btn{
position:fixed;
right:30px;
bottom:30px;
background:var(--secondary);
color:white;
width:45px;
height:45px;
border-radius:50%;
display:flex;
align-items:center;
justify-content:center;
text-decoration:none;
}

/* Responsive */

@media(max-width:900px){

.sidebar{
position:relative;
width:100%;
height:auto;
}

.main{
margin-left:0;
}

}

</style>
</head>

<body>

<!-- Sidebar -->

<div class="sidebar">

<h2>មាតិកាសារណា</h2>

<a href="#cover">ទំព័រមុខ</a>
<a href="#intro">ជំពូក១</a>
<a href="#hr">ជំពូក២</a>
<a href="#district">ជំពូក៣</a>
<a href="#analysis">ជំពូក៤</a>
<a href="#conclusion">ជំពូក៥</a>

</div>

<!-- Content -->

<div class="main">

<!-- Cover -->

<section id="cover" class="section" style="text-align:center">

<h2 style="font-family:'Khmer OS Muol Light';color:var(--primary)">
សាកលវិទ្យាល័យឥន្ទ្រវិជ្ជា
</h2>

<h3 style="color:var(--secondary)">
មហាវិទ្យាល័យពាណិជ្ជសាស្ត្រ និងសេដ្ឋកិច្ច
</h3>

<br>

<h2>
«ការគ្រប់គ្រង និងអភិវឌ្ឍន៍ធនធានមនុស្ស ក្នុងវិស័យរដ្ឋបាលសាធារណៈ»
</h2>

<br>

<p>សារណាបញ្ចប់ការសិក្សា</p>
<p>ឆ្នាំសិក្សា ២០២៤-២០២៥</p>

</section>

<!-- Chapter 1 -->

<section id="intro" class="section">

<h2 class="title">ជំពូកទី១ សេចក្តីផ្តើម</h2>

<p>

ការសិក្សាស្រាវជ្រាវនេះមានគោលបំណងសិក្សាពីការគ្រប់គ្រងធនធានមនុស្ស
ក្នុងរដ្ឋបាលសាធារណៈ និងការអភិវឌ្ឍសមត្ថភាពមន្ត្រី។

</p>

</section>

<!-- Chapter 2 -->

<section id="hr" class="section">

<h2 class="title">ជំពូកទី២ ស្ថានភាពធនធានមនុស្ស</h2>

<table>

<tr>
<th>ការិយាល័យ</th>
<th>ចំនួន</th>
<th>ស្រី</th>
</tr>

<tr>
<td>រដ្ឋបាល</td>
<td>8</td>
<td>3</td>
</tr>

<tr>
<td>OWSO</td>
<td>7</td>
<td>4</td>
</tr>

<tr>
<td>ដែនដី</td>
<td>6</td>
<td>1</td>
</tr>

</table>

<div class="chart-box">
<canvas id="eduChart"></canvas>
</div>

</section>

<!-- Chapter 3 -->

<section id="district" class="section">

<h2 class="title">ជំពូកទី៣ ស្ថានភាពស្រុក</h2>

<iframe
src="https://www.google.com/maps?q=10.5114,104.3315&output=embed"
width="100%"
height="400"
style="border:0">
</iframe>

<div class="chart-box">
<canvas id="popChart"></canvas>
</div>

</section>

<!-- Chapter 4 -->

<section id="analysis" class="section">

<h2 class="title">ជំពូកទី៤ វិភាគ</h2>

<div class="chart-box">
<canvas id="barChart"></canvas>
</div>

</section>

<!-- Chapter 5 -->

<section id="conclusion" class="section">

<h2 class="title">ជំពូកទី៥ សន្និដ្ឋាន</h2>

<p>

ការសិក្សាបង្ហាញថា ការគ្រប់គ្រងធនធានមនុស្សមានសារៈសំខាន់
ក្នុងការកែលម្អប្រសិទ្ធភាពសេវាសាធារណៈ។

</p>

</section>

</div>

<a href="#" class="top-btn">
<i class="fas fa-arrow-up"></i>
</a>

<script>

/* Education Chart */

new Chart(document.getElementById("eduChart"),{

type:'doughnut',

data:{
labels:['បរិញ្ញាបត្រ','បរិញ្ញាបត្ររង','អនុបណ្ឌិត','មធ្យម'],

datasets:[{
data:[26,10,3,5],
backgroundColor:[
'#003366',
'#cc0000',
'#d4af37',
'#718096'
]
}]
}

});


/* Population Chart */

new Chart(document.getElementById("popChart"),{

type:'line',

data:{
labels:['២០២១','២០២២','២០២៣','២០២៤','២០២៥'],

datasets:[{

label:'ប្រជាជន',

data:[14200,14800,15500,16300,17500],

borderColor:'#003366',

fill:false

}]

}

});


/* Comparison */

new Chart(document.getElementById("barChart"),{

type:'bar',

data:{
labels:['តម្លាភាព','ល្បឿន','វិជ្ជាជីវៈ','IT'],

datasets:[

{
label:'មុន',
data:[35,30,45,20],
backgroundColor:'#ccc'
},

{
label:'បច្ចុប្បន្ន',
data:[85,75,80,55],
backgroundColor:'#003366'
}

]

}

});

</script>

</body>
</html>
