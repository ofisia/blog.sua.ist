---
title: "Dsbl Btwrdn Pdts."
datePublished: Tue Aug 26 2025 08:29:58 GMT+0000 (Coordinated Universal Time)
cuid: cmesacked000402jvhc2hdl39
slug: dsbl-btwrdn-pdts

---

Setelah sempat putus asa pada [minggu lalu](https://blog.sua.ist/whabitsta), kini saya telah menemukan cara untuk menonaktifkan pemutakhiran otomatis [Bitwarden](https://bitwarden.com/). Urutan langkahnya sederhana saja sebenarnya, cukup hanya bermodalkan [Terminal](https://en.wikipedia.org/wiki/Terminal_\(macOS\)). Untuk *posterity*, saya akan mencatatnya disini.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1756196970817/acb7a134-720b-4e4a-a98c-55d3d2dabca2.png align="center")

([sumber gambar](https://publicdomainreview.org/collection/serviette-sculptures-the-forgotten-art-of-napkin-folding/))

1. Buka Terminal.
    
2. Tempel `defaults write com.bitwarden.desktop SquirrelAutomaticallyUpdate -bool NO` untuk menonaktifkan.
    
3. Buka ulang Bitwarden.
    
4. Tempel `defaults read com.bitwarden.desktop SquirrelAutomaticallyUpdate` untuk memeriksa ulang nonaktifasi.
    
5. Jika *output* menampilkan angka `0` maka berarti `false` *a.k.a.* pemutakhiran otomatis telah nonaktifkan.
    

Baiklah, demikian saudara-saudari, pestanya bubar. Saatnya kembali ke rutinitas awal, dengan Bitwarden versi usang, tapi yang penting masih bisa dipakai. Karena *updates* adalah untuk *poseurs*.

([sua](https://sua.ist))