# BelajarAndroid3_MembuatMaps
Ini adalah project latihan android saya ke-3 yang saya upload ke github

# Introduction
Assalamu'alaykum Warrohmatullahi Wabarokatuh. Hello sob!
Pada kesempatan kali ini saya disini membagikan hasil project kecil-kecilan saya. walaupun ini sangat sederhana dibandingkan project sobat yang luar biasa itu tapi semoga ini menjadikan proses saya belajar dan menjadi motivasi agar terus membuat project yang lebih kompleks dan besar lagi.

Ini file project membuat Maps di android dengan titik utama nya di Bogor. sobat jika ingin mengganti cukup ganti titik utama mapsnya sesuai kota sobat di bagian MapsActivity.

    
    @Override
    public void onMapReady(GoogleMap googleMap) {
        mMap = googleMap;

        // Add a marker in Sydney and move the camera
        LatLng bogor = new LatLng(-6.595038, 	106.816635);
        mMap.addMarker(new MarkerOptions().position(bogor).title("Marker in bogor"));
        mMap.moveCamera(CameraUpdateFactory.newLatLng(bogor));
    }

Sobat tinggal mengganti Latitude dan Longitude berdasarkan kota sobat. bagaimana cara mengetahuinya kak? gampang sekali, sobat cukup ketikkan di google Latitude dan Longitude kota sobat kemudian sobat Copy Paste disana.

# Installation
Sobat cukup Clone atau Donwload dan buka di Android Studio untuk

    https://github.com/yummicodes/BelajarAndroid3_MembuatMaps


atau cara kedua yaitu sobat dapat menggunakan [DownGit](https://downgit.github.io/#/home) untuk mendownload ini, salin dibawah ini

    https://github.com/yummicodes/BelajarAndroid3_MembuatMaps
dan Tempel ke DownGit, setelah itu klik Tombol Unduh, dan Selamatt, Anda dapat mengkloning kodenya.

Kemudian yang tidak kalah pentingnya sobat ubah API KEY nya

    <string name="google_maps_key" templateMergeStrategy="preserve" translatable="false">REPLACE YOUR API KEY HERE!!</string>
    
Disana tertulis "REPLACE YOUR API KEY HERE!!" yang harus sobat ganti. caranya mendapatakannya adalah dengan mengunjungi link [ini](https://console.cloud.google.com/apis/api). sobat nanti silahkan buat API nya kemudian nnati di Replace ke sana
