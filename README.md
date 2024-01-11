# Multiple Java Version
---

## **Step 1** - Download dan Install JDK
Download versi JDK yang akan digunakan, misal kita akan menggunakan 3 versi Java seperti Java 8, Java 11, dan Java 17. 

## **Step 2** - Set up JDK kedalam Environment Variables
Cukup masukan salah satu JDK yang akan dijadikan sebagai default versi Java.

## **Step 3** - Download Script untuk mengubah versi Java
Untuk mengubah versi Java melalui CLI tanpa harus mengubah settingan Environment Variables, silahkan clone Repository ini untuk mendapatkan scripts-nya atau [Klik disini](https://www.happycoders.eu/wp-content/uploads/2023/04/scripts-up-to-java21.zip).

## **Step 4** - Edit kedua file javaX
- Sesuaikan lokasi File JDK yang ada di file `javaX.bat`
```
if %1 == "Java 1.2" set JAVA_HOME=C:\Program Files (x86)\Java\jdk1.2.2
if %1 == "Java 1.3" set JAVA_HOME=C:\Program Files (x86)\Java\jdk1.3.1_28
if %1 == "Java 1.4" set JAVA_HOME=C:\Program Files (x86)\Java\jdk1.4.2_19
if %1 == "Java 5" set JAVA_HOME=C:\Program Files (x86)\Java\jdk1.5.0_22
if %1 == "Java 6" set JAVA_HOME=C:\Program Files\Java\jdk1.6.0_45
if %1 == "Java 7" set JAVA_HOME=C:\Program Files\Java\jdk1.7.0_80
if %1 == "Java 8" set JAVA_HOME=C:\Program Files\Java\jdk1.8.0_291
if %1 == "Java 9" set JAVA_HOME=C:\Program Files\Java\jdk-9.0.4
if %1 == "Java 10" set JAVA_HOME=C:\Program Files\Java\jdk-10.0.2
if %1 == "Java 11" set JAVA_HOME=C:\Program Files\Java\jdk-11.0.11
if %1 == "Java 12" set JAVA_HOME=C:\Program Files\Java\jdk-12.0.2
if %1 == "Java 13" set JAVA_HOME=C:\Program Files\Java\jdk-13.0.2
if %1 == "Java 14" set JAVA_HOME=C:\Program Files\Java\jdk-14.0.2
if %1 == "Java 15" set JAVA_HOME=C:\Program Files\Java\jdk-15.0.2
if %1 == "Java 16" set JAVA_HOME=C:\Program Files\Java\jdk-16.0.2
if %1 == "Java 17" set JAVA_HOME=C:\Program Files\Java\jdk-17.0.6+10
if %1 == "Java 18" set JAVA_HOME=C:\Program Files\Java\jdk-18
if %1 == "Java 19" set JAVA_HOME=C:\Program Files\Java\jdk-19
if %1 == "Java 20" set JAVA_HOME=C:\Program Files\Java\jdk-20
if %1 == "Java 21" set JAVA_HOME=C:\Program Files\Java\jdk-21
```

- Sesuaikan juga lokasi File JDK yang ada di file `javaX.ps1`
```
	"Java 1.2" { $env:JAVA_HOME = "C:\Program Files (x86)\Java\jdk1.2.2" }
	"Java 1.3" { $env:JAVA_HOME = "C:\Program Files (x86)\Java\jdk1.3.1_28" }
	"Java 1.4" { $env:JAVA_HOME = "C:\Program Files (x86)\Java\jdk1.4.2_19" }
	"Java 5" { $env:JAVA_HOME = "C:\Program Files (x86)\Java\jdk1.5.0_22" }
	"Java 6" { $env:JAVA_HOME = "C:\Program Files\Java\jdk1.6.0_45" }
	"Java 7" { $env:JAVA_HOME = "C:\Program Files\Java\jdk1.7.0_80" }
	"Java 8" { $env:JAVA_HOME = "C:\Program Files\Java\jdk1.8.0_291" }
	"Java 9" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-9.0.4" }
	"Java 10" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-10.0.2" }
	"Java 11" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-11.0.11" }
	"Java 12" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-12.0.2" }
	"Java 13" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-13.0.2" }
	"Java 14" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-14.0.2" }
	"Java 15" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-15.0.2" }
	"Java 16" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-16.0.2" }
	"Java 17" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-17.0.6+10" }
	"Java 18" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-18" }
	"Java 19" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-19" }
	"Java 20" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-20" }
	"Java 21" { $env:JAVA_HOME = "C:\Program Files\Java\jdk-21" }
```

## **Step 5** : Tambahkan direktori scripts kedalam Environmet Variables

Setelah menambahkan folder scripts kedalam Environment Variables sekarang kita bisa mengubah versi Java melalui CLI. 

- **Merubah sementara versi Java** jalankan `java<versi>`, contoh `java11`. Setelah dijalankan versi Java akan berubah, tetapi jika CLI diclose maka versi Java akan kembali ke semula sesuai versi pada Environment Variables.

- **Merubah permanen versi Java** jalankan `java<versi> perm`, contoh `java11 perm`. Setelah dijalankan versi Java akan berubah dan tidak akan kembali ke semula walaupun CLI sudah diclose.


