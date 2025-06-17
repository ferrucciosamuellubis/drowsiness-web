# Drowsiness Detector Web

Web aplikasi deteksi kantuk berbasis **HTML + JavaScript** menggunakan [face-api.js](https://github.com/justadudewhohacks/face-api.js).  
Tidak memerlukan backend/server Python—semua proses berjalan di browser!  
Mendeteksi tanda-tanda kantuk dengan menghitung Eye Aspect Ratio (EAR) dari webcam secara real-time.

---

## 🚀 Demo

Coba secara live setelah deploy ke Vercel/Netlify/GitHub Pages, atau jalankan secara lokal.

---

## 📦 Struktur Project

```
/
├── index.html
└── models/
     ├── tiny_face_detector_model-weights_manifest.json
     ├── tiny_face_detector_model-shard1
     ├── face_landmark_68_tiny_model-weights_manifest.json
     ├── face_landmark_68_tiny_model-shard1
```

---

## ⚙️ Cara Menjalankan Lokal

1. **Clone repo ini:**
   ```bash
   git clone https://github.com/username/drowsiness-detector-web.git
   cd drowsiness-detector-web
   ```

2. **Download model weights face-api.js:**
   - Unduh file berikut dari [face-api.js-models/weights](https://github.com/justadudewhohacks/face-api.js-models/tree/master/weights):
     - `tiny_face_detector_model-weights_manifest.json`
     - `tiny_face_detector_model-shard1`
     - `face_landmark_68_tiny_model-weights_manifest.json`
     - `face_landmark_68_tiny_model-shard1`
   - Simpan semua file ke folder `models/` di root repo (sejajar dengan `index.html`).

3. **Jalankan secara lokal:**
   - Bisa langsung buka `index.html` di browser (klik dua kali), atau gunakan webserver sederhana:
     ```bash
     # Dengan Python 3
     python -m http.server 8000
     # lalu buka http://localhost:8000 di browser
     ```

---

## 🌐 Cara Deploy Gratis

- **Vercel:**  
  Push repo ini ke GitHub, lalu deploy via [Vercel Dashboard](https://vercel.com/).
- **Netlify:**  
  Drag & drop folder ke [Netlify](https://netlify.com/).
- **GitHub Pages:**  
  Aktifkan Pages pada repo, pastikan folder `models/` ikut di-publish.

---

## 🛠️ Fitur

- Deteksi kantuk real-time via webcam (EAR threshold).
- Semua pemrosesan berjalan di browser (tidak ada backend).
- Tampilan modern (TailwindCSS).
- Alarm otomatis dan statistik deteksi.

---

## ✨ Credit

- [face-api.js](https://github.com/justadudewhohacks/face-api.js) untuk deteksi wajah & landmark.
- [TailwindCSS](https://tailwindcss.com/) untuk UI.

---

## 📄 Lisensi

MIT License
