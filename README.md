# mystery_module.py

## Temel İşlev
Bu modül, ikinci dereceden bir denklemin köklerini hesaplamak için kullanılır. `fn_x` fonksiyonu, verilen katsayılar ile ax² + bx + c = 0 denkleminin reel köklerini döndürür.

## Fonksiyonlar

### fn_x(a, b, c)
- **Açıklama:**
  - ax² + bx + c = 0 biçimindeki ikinci dereceden denklemin köklerini hesaplar.
  - Diskriminant (d = b² - 4ac) negatifse, fonksiyon `None` döndürür (reel kök yoktur).
  - Diskriminant sıfır veya pozitifse, iki reel kökü tuple olarak döndürür.
- **Parametreler:**
  - `a` (float/int): x²'nin katsayısı
  - `b` (float/int): x'in katsayısı
  - `c` (float/int): sabit terim
- **Dönüş:**
  - Tuple (kök1, kök2) (her biri float)
  - Reel kök yoksa: `None`

## Kullanım Örneği
```python
from mystery_module import fn_x

# ax² + bx + c = 0 için örnek: x² - 3x + 2 = 0
sonuc = fn_x(1, -3, 2)
print(sonuc)  # (2.0, 1.0)

# Reel kök yoksa
print(fn_x(1, 0, 1))  # None
