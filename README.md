<!DOCTYPE html>
<html>
<head>
<style>
body {
background-color: lightgreen;
}
  
h1 {
color: white;
  text-align: center;
}

h2 {
color: white;
text-align: left;
font-size: 22px;
}

P {
font-family: rallway;
font-size: 18px;
}

</head>
</style>
<body>

<h1>CLEANING SERVICE</h1>
<p>Penyedia Layanan Jasa Cleaning Service di Kota Semarang yang berkualitas, wangi, cepat, dan terjangkau.</p>
<h2> INFO </h2>
<p> Fasilitas kebersihan sudah disediakan oleh pihak layanan jasa, jadi tuan rumah tidak perlu menyiapkan fasilitas lagi. Hasil dari pengerjaan dijamin bersih, wangi, dan cepat. Jika kurang memuaskan, pihak penyedia jasa siap untuk mengoreksi bahkan mengembalikan uang anda 50%.</p>
<h2> SYARAT DAN KETENTUAN</h2>
<p> Pihak customer harus memberi tahu kondisi ruangan yang perlu dibersihkan terlebih dahulu. Jika ada tambahan ruangan, customer bisa menyampaikan setelah pekerjaan pertama selesai dan setelah melakukan pembayaran. Untuk pemesanan, pihak customer diharuskan untuk membayar dp 20% terlebih dahulu sebagai tanda fix order.</p>


</body>
</html>
<h2> FORM PEMESANAN</h2>
<form action="proses-pemesanan.php" method="post">
		<label for="nama">Nama:</label>
  	<input type="text" id="nama" name="nama" required>

		<p><label for="alamat">Alamat:</label>
   	<textarea id="alamat" name="alamat" rows="5" cols="30" required></textarea>

   <p><label for="layanan">Jenis Layanan:</label>
   <select id="layanan" name="layanan">
   <option value="gedung">*pilih</option>
			<option value="rumah">Rumah</option>
			<option value="kantor">Kantor</option>
			<option value="gedung">Apartemen</option>
			<option value="gedung">Aula</option>

		</select>

<p><label><i class="fa fa-room"></i> Jumlah Ruangan</label>
      <input class="w3-input w3-border" type="number" value="1" name="Room" min="1" max="50">

<p><label for="tanggal">Tanggal:</label>
  		<input type="date" id="tanggal" name="tanggal" required>

<p><label for="jam">Jam:</label>
    	<input type="time" id="jam" name="jam" required>
    
<p><label for="layanan">Metode Pembayaran:</label>
<select id="pembayaran" name="lpembayaran">
<option value="gedung">*pilih</option>
			<option value="rumah">Kartu Debit</option>
  		<option value="kantor">Kartu Kredit</option>
     	<option value="gedung">E-wallet</option>
</select>


<p><button class="w3-button w3-block w3-green w3-left-align" class="fa fa-clock-o" type="submit"><i w3-margin-center"></i> Pesan Sekarang</button></p>

<h2>.....................................................................................................................</h2>
<p>Untuk pengaduan layanan dan info lebih lanjut, bisa hubungi kami di:
<p>Telp : +62 1515151112
<p>Email : cleaningservice@gmail.com
<p>Alamat : Jalan Kita Masih Panjang No. 666

	</form>
 	<script>
  		// kode JavaScript untuk validasi form
    	function validateForm() {
      		var nama = document.getElementById("nama").value;
         	var alamat = document.getElementById("alamat").value;
        	var tanggal = document.getElementById("tanggal").value;
        	var jam = document.getElementById("jam").value;

			    if (nama == "" || alamat == "" || tanggal == "" || jam == "") {
   			    	alert("Mohon isi semua field yang diperlukan");
       			 	return false;
          }
      }
		  // panggil fungsi validateForm() ketika form di-submit
  		document.querySelector("form").addEventListener("submit", validateForm);
    	</script>
</body>
</html>
