# GIT BRANCH 
--- 

# 1. POIN UTAMA:
---
 ###  **A. Apa itu git branching?**
 ```
 Git memungkinkan percabangan, membuat garis waktu terpisah untuk pengembangan, mencegah perubahan di satu branch mempengaruhi branch utama.
   
 Percabangan berguna untuk menambahkan fitur baru tanpa mengubah basis kode utama, sehingga pengembang dapat bekerja secara mandiri pada tugas yang berbeda.

 Perintah git seperti "git branch" dan "git checkout" digunakan untuk membuat dan beralih di antara branch.
   
 Branch dapat diganti namanya menggunakan "git branch -m [nama lama] [nama baru]".
   
 Branch yang tidak digunakan dapat dihapus menggunakan "git branch -d [nama branch]".
     
 Beberapa branch adalah hal yang umum dalam pengembangan perangkat lunak, memfasilitasi pekerjaan paralel pada fitur yang berbeda atau perbaikan bug.
```
---

 ###  **B.Merging**
 ```
 - Untuk menggabungkan perubahan dari satu branch ke branch lainnya di Git, alihkan ke branch tujuan dan gunakan perintah "git merge".

 - conflict dapat terjadi di Git ketika beberapa programmer memodifikasi file yang sama di branch yang berbeda, yang membutuhkan perubahan manual.

 - Membuat branch di Git memungkinkan pengembangan paralel dan isolasi fitur, tetapi conflict dapat muncul ketika merging.

 - Conflict dapat diselesaikan secara manual dengan mengedit file yang memiliki conflict, diikuti dengan melakukan commit.
```
---

   ### **C.Cherry Pick**
   ```
 - Cherry-pick memungkinkan untuk memilih commit tertentu dari satu branch dan menerapkannya ke branch lain, berguna ketika Anda hanya ingin menerapkan perubahan tertentu.
 ```
---

  ### D.Tags
 ```
 - Tags di Git adalah referensi untuk commit tertentu, yang sering digunakan untuk menandai versi rilis aplikasi.

 - Tags dapat didaftarkan dan diperiksa untuk menavigasi antara berbagai versi repository, memberikan snapshots pada titik waktu tertentu.

 - Untuk mengubah tags di Git, buat tag baru yang mengarah ke commit yang sama, lalu hapus tag lama.

 - Menghapus tag di Git dapat dilakukan dengan menggunakan perintah "git tag -d <tagname>".
```
---

  ### E.Stash
```
 - Stashing di Git memungkinkan penyimpanan sementara perubahan yang dibuat di Working directory atau staging index.

 - Menyimpan perubahan dilakukan dengan perintah "git stash push -m <pesan>".

 - Untuk membuat daftar semua simpanan, gunakan "git stash list".
   
 - Untuk menerapkan perubahan dari sebuah stash, gunakan git stash apply [stashid].

 - Stash dapat dihapus menggunakan git stash drop [stashid] atau git stash clear.
```
---
  ### F.Rebase
 ```
 - Melakukan "rebase" di Git melibatkan pemindahan ke branch tempat Anda ingin menerapkan perubahan, tidak seperti merging di mana Anda tetap berada di cabang saat ini.

 - Rebase melibatkan penulisan ulang riwayat commit, membuatnya tampak seolah-olah perubahan dibuat langsung pada branch saat ini.

 - Untuk melakukan rebase, gunakan perintah "git rebase <branch-name>", di mana <branch-name> adalah nama branch yang berisi perubahan yang akan diterapkan.

 - Squashing commits di Git melibatkan penggabungan beberapa komit menjadi satu komit untuk riwayat yang lebih bersih.

 - Squashing commits dapat dilakukan selama operasi rebase dengan menggunakan perintah "git rebase -i" dan memilih opsi "squash" untuk commit yang diinginkan.

 - Squashing commits membuat riwayat commit menjadi lebih ringkas, tetapi dapat mengakibatkan hilangnya pesan dan referensi commit individual.

 - Git branching memungkinkan penggabungan beberapa commit menjadi satu dengan menggunakan perintah "squash".
 ```
---
 ###  G.Trunk Based Development
 ```
 - Trunk Based Development menyederhanakan branching dengan hanya satu branch utama, dengan fokus pada pengiriman fitur yang cepat langsung ke produksi setelah pengujian.
```
---
###  H.Forking Workflow
```
   - Forking Workflow adalah hal yang umum dalam project open source, di mana kontributor menduplikasi repositori utama, membuat perubahan dalam fork mereka, dan kemudian meminta perubahan tersebut untuk         digabungkan ke dalam proyek utama.

   - Forking Workflow memungkinkan kolaborasi sambil mempertahankan kontrol atas repositori utama dan memastikan perubahan ditinjau sebelum integrasi.
```

---


 #  2. PERTANYAAN

 >  a) Apakah lebih baik menggunakan squash atau rebase?





#  3. KESIMPULAN

 >  Kesimpulannya, memahami berbagai strategi Branching Git seperti Gitflow, Trunk Based Development, dan Forking Workflow memberikan fleksibilitas kepada pengembang dalam mengelola kontrol versi dan           kolaborasi. Setiap strategi memiliki kelebihan dan cocok untuk berbagai kebutuhan proyek. Baik itu mempertahankan proses pengembangan yang terstruktur, memungkinkan pengiriman fitur yang cepat,
    atau memfasilitasi kontribusi sumber terbuka, memilih strategi percabangan yang tepat sangat penting untuk pengembangan perangkat lunak yang efisien dan efektif.

    
   

   
   

     
