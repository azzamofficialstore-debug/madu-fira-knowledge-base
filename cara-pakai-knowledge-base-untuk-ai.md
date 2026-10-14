<!--
Knowledge Base — Sistem · Nakama SOP Playbook
Dokumen: Cara Pakai Knowledge Base Ini untuk AI
Dipakai untuk: SOP Agent AI
Catatan: file ini adalah standar/SOP yang bisa dipakai sebagai konteks untuk AI agent / automation.
-->

# Cara Pakai Knowledge Base Ini untuk AI

Knowledge base ini bukan cuma bacaan tim. Tiap file `.md` dirancang jadi **satu unit konteks yang berdiri sendiri**, sehingga bisa langsung dimasukkan ke AI tanpa perlu banyak penjelasan tambahan.

## Prinsip

- **Satu file = satu topik.** Jangan menggabung banyak SOP dalam satu prompt kalau tidak perlu — beri AI file yang paling relevan dengan tugasnya.
- **File ini adalah "aturan main", bukan sekadar informasi.** Perlakukan isinya sebagai standar yang harus dipatuhi AI saat membuat/mereview output.
- **Selalu tambahkan konteks brand.** Knowledge base ini generik (standar Nakama). Sebelum AI bekerja, lengkapi dengan konteks brand spesifik (lihat folder Reference & Context).

## Tiga cara memakainya

1. **Sebagai system prompt / custom instruction.** Tempel isi file ke bagian "instructions" AI agent atau custom GPT. Cocok untuk SOP dan Standar (mis. Definition of Done, do's & don'ts).
2. **Sebagai knowledge / file attachment.** Unggah beberapa file `.md` ke AI yang mendukung retrieval (mis. custom GPT knowledge, vector store, project files). AI akan merujuknya saat relevan.
3. **Sebagai konteks sekali pakai.** Tempel satu file di awal chat, lalu minta AI mengerjakan tugas berdasarkan standar itu.

## Pola prompt yang disarankan

> "Kamu adalah asisten [ROLE] di tim sosial media. Ikuti standar berikut apa adanya. Kalau ada yang tidak sesuai standar, tandai. Standar: [tempel isi file]. Tugas: [tugasmu]."

## Yang perlu diingat

- **AI tetap butuh checkpoint manusia.** Standar di sini menaikkan lantai kualitas, bukan menggantikan review akhir.
- **Perbarui saat SOP berubah.** Kalau standar tim berubah, unduh ulang file terbaru — jangan biarkan AI memakai versi lama.
- **Jangan bocorkan data sensitif.** File ini standar proses, bukan tempat menaruh rahasia brand/klien.
