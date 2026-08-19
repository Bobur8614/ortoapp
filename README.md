# Orto

**Orto** — jarohat/jarrohlikdan keyingi reabilitatsiya va mashqlar dasturini boshqarish uchun mo'ljallangan Android ilova. Foydalanuvchiga shaxsiy reabilitatsiya dasturi, kunlik mashqlar, progress kuzatuvi hamda mutaxassis bilan muloqot imkoniyatini beradi.

> **Eslatma:** Bu repozitoriyda hozircha faqat tayyor `Orto.apk` fayli va IDE (`.idea`) konfiguratsiyasi mavjud — ilovaning manba kodi (source code) hali repoga qo'shilmagan. Quyidagi tavsif APK faylini (manifest, resurslar, klass nomlari) tahlil qilish orqali aniqlangan, shuning uchun ba'zi tafsilotlar taxminiy bo'lishi mumkin.

## Asosiy imkoniyatlar

APK tarkibidagi ma'lumotlar (DTO va klass nomlari) asosida aniqlangan funksiyalar:

- **Ro'yxatdan o'tish / kirish** — telefon raqami orqali ro'yxatdan o'tish, SMS/OTP orqali tasdiqlash, parolni unutish va tiklash
- **Profil** — jins, viloyat/tuman kabi ma'lumotlarni to'ldirish
- **Reabilitatsiya dasturlari** — dashboard, mashqlar (mashq va uning bosqichlari), kunlik reabilitatsiya kunlari, progress va snapshot (kesma) ko'rinishidagi kuzatuv
- **Individual dastur va progress** — foydalanuvchiga biriktirilgan dastur va uning bajarilish holati
- **Jadval** — mashqlar jadvali va offline holatda ham ishlaydigan sinxronizatsiya
- **Yutuqlar (achievements)** — gamifikatsiya elementlari
- **Chat** — mutaxassis/shifokor bilan yozishmalar (xabarni tahrirlash imkoniyati bilan)
- **To'lov** — dasturlarni sotib olish (checkout, xarid oldindan ko'rish)
- **Bildirishnomalar** — Firebase orqali push-xabarlar hamda qurilma qayta yoqilgandan keyin ham ishlaydigan rejalashtirilgan eslatmalar
- **Ko'p tillilik** — interfeys bir nechta tilni qo'llab-quvvatlaydi

## Texnologiyalar

- Kotlin + Jetpack Compose / Compose Multiplatform
- Ktor — tarmoq so'rovlari uchun HTTP klient
- kotlinx.serialization, kotlinx.coroutines
- AndroidX DataStore — lokal sozlamalarni saqlash
- Coil3 — rasmlarni yuklash va keshlash
- Firebase Cloud Messaging — push-bildirishnomalar
- Google Play Services

## Texnik ma'lumotlar

| | |
|---|---|
| Paket nomi | `uz.ilkhom.orto` |
| Asosiy activity | `uz.ilkhom.orto.MainActivity` |
| Versiya | 1.1 |
| Qo'llab-quvvatlanadigan arxitekturalar | `arm64-v8a`, `armeabi-v7a`, `x86`, `x86_64` |

## Yuklab olish

Eng so'nggi versiya: **[Orto.apk — GitHub Releases](https://github.com/Bobur8614/ortoapp/releases/latest)**

## O'rnatish

1. Yuqoridagi havoladan `Orto.apk` faylini yuklab oling.
2. Android qurilmangizda noma'lum manbalardan o'rnatishga ruxsat bering.
3. `Orto.apk` faylini oching va o'rnatishni yakunlang.

## Ruxsatlar

Ilova quyidagi asosiy ruxsatlardan foydalanadi: internet va tarmoq holatini tekshirish, bildirishnomalarni yuborish, aniq vaqtda signal (eslatma) rejalashtirish va qurilma qayta yoqilganda eslatmalarni tiklash.
