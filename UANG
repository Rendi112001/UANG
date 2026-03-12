<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Manajemen Keuangan</title>
<style>
body{
    font-family: Arial, sans-serif;
    margin:0;
    background:#f4f6f9;
}

header{
    background:#2c7be5;
    color:white;
    padding:20px;
    text-align:center;
}

.container{
    width:90%;
    max-width:900px;
    margin:auto;
    margin-top:20px;
}

.card{
    background:white;
    padding:20px;
    border-radius:10px;
    box-shadow:0 2px 5px rgba(0,0,0,0.1);
    margin-bottom:20px;
}

input, select, button{
    padding:10px;
    margin:5px 0;
    width:100%;
}

button{
    background:#2c7be5;
    color:white;
    border:none;
    cursor:pointer;
}

button:hover{
    background:#1a5ec8;
}

table{
    width:100%;
    border-collapse:collapse;
}

th, td{
    padding:10px;
    border-bottom:1px solid #ddd;
    text-align:left;
}

.pemasukan{
    color:green;
}

.pengeluaran{
    color:red;
}
</style>
</head>
<body>

<header>
<h1>Web Manajemen Keuangan</h1>
<p>Catat pemasukan dan pengeluaran kamu</p>
</header>

<div class="container">

<div class="card">
<h2>Tambah Transaksi</h2>

<input type="text" id="deskripsi" placeholder="Deskripsi">

<input type="number" id="jumlah" placeholder="Jumlah uang">

<select id="tipe">
<option value="pemasukan">Pemasukan</option>
<option value="pengeluaran">Pengeluaran</option>
</select>

<button onclick="tambahData()">Tambah</button>
</div>

<div class="card">
<h2>Riwayat Keuangan</h2>

<table>
<thead>
<tr>
<th>Deskripsi</th>
<th>Jumlah</th>
<th>Tipe</th>
</tr>
</thead>

<tbody id="dataKeuangan"></tbody>

</table>
</div>

</div>

<script>
function tambahData(){

let deskripsi = document.getElementById("deskripsi").value;
let jumlah = document.getElementById("jumlah").value;
let tipe = document.getElementById("tipe").value;

if(deskripsi=="" || jumlah==""){
alert("Isi semua data");
return;
}

let tabel = document.getElementById("dataKeuangan");

let row = tabel.insertRow();

row.insertCell(0).innerText = deskripsi;
row.insertCell(1).innerText = "Rp " + jumlah;

let tipeCell = row.insertCell(2);
tipeCell.innerText = tipe;

if(tipe=="pemasukan"){
tipeCell.className="pemasukan";
}else{
tipeCell.className="pengeluaran";
}

document.getElementById("deskripsi").value="";
document.getElementById("jumlah").value="";
}
</script>

</body>
</html>
