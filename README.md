# Point in Polygon - Parallel Programming 🎯

Bu proje, rastgele oluşturulan devasa bir çokgenin (poligonun) içine düşen noktaları tespit eden **Ray Casting (Işın Dökümü)** algoritmasının, Java kullanılarak paralelleştirilmiş çözümünü içermektedir.

## 🚀 Özellikler

* **Ray Casting Algoritması:** Matematiksel doğru-çizgi kesişim mantığı ile kusursuz nokta-poligon testi.
* **Multithreading (Çoklu İş Parçacığı):** Java `ExecutorService` ve `AtomicInteger` kullanılarak sistemdeki tüm işlemci çekirdeklerinin (örneğin 16 Thread) asenkron olarak kullanılması.
* **Dinamik Performans Ölçümü:** Seri (tek çekirdek) ve Paralel (çoklu çekirdek) çalışma sürelerinin karşılaştırılarak **Hızlanma Katsayısının (Speedup)** otomatik hesaplanması.

## 🛠️ Kurulum ve Çalıştırma

Projeyi çalıştırmak için sisteminizde **Java 17 veya üzeri** yüklü olmalıdır.

1. Projeyi bilgisayarınıza klonlayın:
   ```bash
       git clone [https://github.com/MATEXIEL/PointInPolygon-BTUParallelProgramming.git](https://github.com/MATEXIEL/PointInPolygon-BTUParallelProgramming.git)

2. IntelliJ IDEA veya tercih ettiğiniz bir IDE ile projeyi açıp `src/Main.java` dosyasını çalıştırabilirsiniz.
3. Alternatif olarak, derlenmiş `.jar` dosyasını terminal üzerinden doğrudan çalıştırabilirsiniz:
```bash
java -jar PointInPolygon.jar

```



## 📊 Deneysel Sonuçlar

Testler (AMD Ryzen 7 6800H - 16 Thread) sonucunda, artan iş yüküyle birlikte paralelleştirmenin gücü ortaya çıkmış; ağır yük altında (50.000 kenarlı poligon ve 500.000 test noktası) yaklaşık **~6 kat (5.98x) hızlanma** elde edilmiştir.
