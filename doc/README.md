## EternalBlue (MS17-010)

EternalBlue (MS17-010) adalah eksploitasi yang ditemukan dalam protokol SMBv1 (Server Message Block version 1) di sistem operasi Windows. Exploit ini memanfaatkan kerentanan dalam cara Windows menangani paket SMB, yang memungkinkan penyerang untuk mengeksekusi kode berbahaya secara remote tanpa perlu autentikasi.

## Detail Teknis

- CVE: CVE-2017-0144
- Ditemukan oleh: NSA (National Security Agency) dan kemudian bocor oleh grup peretas Shadow Brokers pada April 2017.

## Target Sasaran

- Windows Vista
- Windows 7
- Windows 8
- Windows 10
- Windows Server 2003
- Windows Server 2008
- Windows Server 2008 R2
- Windows Server 2012
- Windows Server 2016

## Cara kerja

Mengeksploitasi cara SMBv1 menangani paket yang dikirim ke port 445, memungkinkan eksekusi kode jarak jauh (Remote Code Execution - RCE).

## Dampak

EternalBlue digunakan dalam berbagai serangan besar, termasuk:

- WannaCry (2017) → Ransomware yang menyebar secara global dalam waktu singkat.
- NotPetya (2017) → Malware yang menyerang sistem keuangan dan perusahaan besar.
- TrickBot & Emotet → Malware yang menggunakan EternalBlue untuk penyebaran.

## Mitigasi dan Pencegahan

- Patch Windows: Microsoft merilis patch MS17-010 pada 14 Maret 2017 untuk memperbaiki kerentanan ini.
- Nonaktifkan SMBv1: Jika tidak diperlukan, matikan protokol SMBv1 di Windows.
- Gunakan firewall: Blokir akses ke port 445 dari jaringan luar.
- Gunakan IDS/IPS: Sistem deteksi intrusi dapat mencegah eksploitasi ini.
