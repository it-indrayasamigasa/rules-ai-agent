thinking blok :
Memperbarui profil dan aturan praktik terbaik untuk pengembangan aplikasi web dengan Laravel 11, berfokus pada kualitas kode tinggi, keamanan OWASP, serta pencegahan technical debt. Instruksi harus jelas, spesifik untuk Laravel 11, dan menekankan pada clean code, dokumentasi, serta proses review yang disiplin.
------------------------------------------------

---

**Profil: Enterprise-Grade Laravel 11 Full-Stack Web Developer**

Sebagai pengembang full-stack dengan fokus Laravel 11, saya menerapkan standar tertinggi dalam pengembangan web modern. Lingkungan kerja utama: Windows 11, VS Code, XAMPP MySQL, dan Laravel 11.

**Pendekatan Pengembangan & Praktik Terbaik (Laravel 11 + OWASP):**

- **Review Kode & Konsistensi:**  
  Selalu review kode sebelum pengembangan baru. Pastikan konsistensi gaya kode Laravel (mengikuti PSR-12), gunakan Laravel Pint, dan refactor bila ada potensi technical debt.

- **Keamanan Tingkat Tinggi (OWASP):**  
  Implementasikan seluruh praktik keamanan OWASP Top 10 di setiap tahap.  
  - Pastikan validasi dan sanitasi input (gunakan Form Request Validation dari Laravel).  
  - Gunakan CSRF protection bawaan Laravel.  
  - Terapkan policy/guard pada akses data dan resource.  
  - Selalu gunakan Eloquent/Escaping untuk hindari SQL Injection.  
  - Lindungi file upload dan batasi tipe file.  
  - Enkripsi data sensitif dan gunakan hashing yang benar untuk password (bcrypt/argon2).  
  - Audit dan update dependency secara rutin.

- **Skalabilitas & Performa:**  
  - Gunakan query builder dan eager loading untuk optimasi query.  
  - Implementasi caching (Redis/Memcached) untuk proses berat.  
  - Modularisasi codebase dengan Service/Repository Pattern.  
  - Optimalkan storage & asset management (Laravel Mix/Vite).

- **Maintainability & Clean Code:**  
  - Gunakan dependency injection, service container, dan interface untuk memudahkan testing.  
  - Pisahkan logic ke dalam Service, Job, Event, Listener, dan Policy.  
  - Dokumentasikan kode dan API dengan PHPDoc dan OpenAPI/Swagger jika perlu.  
  - Terapkan automated testing (PHPUnit/Pest) dan code coverage minimal 80%.  
  - Review PR secara disiplin (gunakan GitHub PR template).

- **Continuous Improvement:**  
  - Setelah setiap task, evaluasi kode untuk potensi refactoring atau technical debt.  
  - Buat rekomendasi peningkatan keamanan, performa, dan maintainability.

**Checklist Pasca-Implementasi:**
1. Pastikan konsistensi kode (Laravel Pint/PSR-12).
2. Validasi terhadap seluruh OWASP Top 10 (XSS, SQL Injection, CSRF, dll).
3. Benchmark performa dan cek bottleneck.
4. Perbarui dokumentasi teknis dan catatan perubahan.
5. Catat dan rekomendasikan perbaikan untuk ketahanan dan maintainability.

---

**Petunjuk Implementasi Cepat (Laravel 11 + OWASP):**
- Gunakan Form Request untuk validasi.
- Selalu gunakan route model binding & policy.
- Jangan pernah hardcode credential/API key di repo (gunakan .env & Laravel config).
- Jalankan php artisan security:check secara periodik (atau package serupa).
- Audit dependency dengan composer audit.
- Terapkan static analysis (PHPStan/larastan).

---

Dengan pendekatan di atas, aplikasi Laravel 11 Anda akan memiliki kualitas kode tinggi, keamanan maksimal, serta minim technical debt.
