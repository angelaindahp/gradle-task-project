📜 Rincian Pengerjaan Tugas
Berikut adalah langkah-langkah rinci yang telah dilakukan dalam tugas ini:

1️⃣ Setup Proyek Java dengan Gradle
Membuat proyek Java di IntelliJ IDEA.
Menggunakan Gradle sebagai sistem build.
Menambahkan konfigurasi build.gradle :

plugins {
    id 'java'
}

group = 'org.angel'
version = '1.0-SNAPSHOT'

repositories {
    mavenCentral()
}

tasks.register('greetingTask') {
    doLast {
        String nama = project.hasProperty('nama') ? project.property('nama') : 'Gradle User'
        println "Hello, angel! Welcome to Gradle World!"
    }
}

dependencies {
    implementation 'com.google.guava:guava:29.0-jre'
    testImplementation 'junit:junit:4.13'
}

test {
    useJUnitPlatform()
}

2️⃣ Mengelola Versi Kontrol dengan Git
Inisialisasi Git di proyek dengan:

git init
git add .
git commit -m "Initial commit"

git remote add origin https://github.com/angelaindahp/gradle-task-project.git
git push -u origin master

git branch -M main
git push -u origin main

3️⃣ Upload Proyek ke GitHub & Merge Branch
Mengunggah proyek ke GitHub dengan git push origin main.
Melakukan perbandingan (compare) antara branch main dan master di GitHub.
Membuat Pull Request (PR) jika diperlukan.
Melakukan merge branch setelah memastikan tidak ada konflik.

4️⃣ Menambahkan README.md
README.md dibuat untuk menjelaskan proyek

# Gradle Custom Task Project

Proyek ini adalah contoh implementasi **Gradle Custom Task** dalam proyek Java.

## 📌 Fitur:
- Menggunakan **Gradle** sebagai sistem build.
- Memiliki **custom task** bernama `greetingTask`.
- Dependensi dikelola dengan **Maven Central**.

## 🔧 Cara Menjalankan:
Jalankan perintah berikut untuk mengeksekusi custom task:
```bash
./gradlew greetingTask

/gradle-custom-task-new
 ├── src/main/java/org/angel/Main.java
 ├── build.gradle
 ├── .gitignore
 ├── settings.gradle
 ├── README.md


---

### **📌 Hasil Akhir**
🎯 **Proyek Gradle berhasil dikonfigurasi dengan custom task.**  
🎯 **Repository GitHub sudah berisi kode proyek, branch `main` dan `master`**  
🎯 **README.md sudah ditambahkan untuk menjelaskan proyek.**  

---

### **📝 Kesimpulan**
✅ **Tugas ini membantu memahami penggunaan Gradle, Git, dan GitHub secara terintegrasi.**  
✅ **Dengan adanya README.md, proyek lebih mudah dipahami oleh orang lain.**  
✅ **Proyek telah berhasil dikembangkan dan diunggah ke GitHub dengan struktur yang rapi.**  

---
