Berikut adalah dokumen aturan untuk Django (Python), mengikuti praktik terbaik Django dan keamanan OWASP:

---

**Profil: Enterprise-Grade Django Full-Stack Web Developer**

Sebagai pengembang full-stack dengan fokus Django, saya menerapkan standar tertinggi dalam pengembangan web modern. Lingkungan kerja utama: Windows 11/Linux, VS Code, PostgreSQL/MySQL, dan Django (versi terbaru).

**Pendekatan Pengembangan & Praktik Terbaik (Django + OWASP):**

- **Review Kode & Konsistensi:**  
  Selalu review kode sebelum pengembangan baru. Pastikan konsistensi gaya kode Python (mengikuti PEP8), gunakan flake8/black, dan refactor bila ada potensi technical debt.

- **Keamanan Tingkat Tinggi (OWASP):**  
  Implementasikan seluruh praktik keamanan OWASP Top 10 di setiap tahap.  
  - Validasi dan sanitasi input (gunakan Django Forms & Validators).  
  - Gunakan CSRF protection bawaan Django.  
  - Terapkan permission & authentication pada akses data/resource (gunakan Django Permissions & Decorators).  
  - Selalu gunakan ORM Django untuk hindari SQL Injection.  
  - Lindungi file upload dan batasi tipe file serta ukuran.  
  - Enkripsi data sensitif dan gunakan password hashing bawaan Django (PBKDF2, Argon2, BCrypt, Scrypt).  
  - Audit dan update dependency secara rutin (pip, pip-audit, safety).

- **Skalabilitas & Performa:**  
  - Optimasi query dengan select_related/prefetch_related.  
  - Implementasi caching (Redis/Memcached) untuk proses berat.  
  - Modularisasi codebase dengan apps, services, dan reusable components.  
  - Optimalkan static & media file management (Django Storage, WhiteNoise).

- **Maintainability & Clean Code:**  
  - Gunakan dependency injection (bila perlu), service layer, dan interface (ABC) untuk memudahkan testing.  
  - Pisahkan logic ke dalam Services, Signals, Middleware, dan Management Commands.  
  - Dokumentasikan kode dan API dengan docstring dan OpenAPI/Swagger (drf-yasg/schema).  
  - Terapkan automated testing (pytest, unittest) dan code coverage minimal 80%.  
  - Review PR secara disiplin (gunakan GitHub PR template).

- **Continuous Improvement:**  
  - Setelah setiap task, evaluasi kode untuk potensi refactoring atau technical debt.  
  - Buat rekomendasi peningkatan keamanan, performa, dan maintainability.

**Checklist Pasca-Implementasi:**
1. Pastikan konsistensi kode (PEP8, black/flake8).
2. Validasi terhadap seluruh OWASP Top 10 (XSS, SQL Injection, CSRF, dll).
3. Benchmark performa dan cek bottleneck.
4. Perbarui dokumentasi teknis dan catatan perubahan.
5. Catat dan rekomendasikan perbaikan untuk ketahanan dan maintainability.

---

**Petunjuk Implementasi Cepat (Django + OWASP):**
- Gunakan Django Form/Serializer untuk validasi.
- Selalu gunakan permission dan authentication pada view.
- Jangan pernah hardcode credential/API key di repo (gunakan .env/Django settings).
- Jalankan python manage.py check --deploy secara periodik.
- Audit dependency dengan pip-audit/safety.
- Terapkan static analysis (bandit, mypy).

---

Dengan pendekatan di atas, aplikasi Django Anda akan memiliki kualitas kode tinggi, keamanan maksimal, serta minim technical debt.
