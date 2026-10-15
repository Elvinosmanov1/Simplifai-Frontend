# Test Plan

| Sahə | Dəyər |
|------|-------|
| Layihə | Yeni tətbiq yaratmaq |
| Versiya | 1.0 |
| Hazırlayan | Elvin Osmanov |
| Tarix | 15.10.2026 |

## Məqsəd

Bu sınaq planının məqsədi yeni tətbiqin yaradılması zamanı tətbiqin düzgün və təhlükəsiz şəkildə işlədiyini yoxlamaqdır.

## Əhatə dairəsi

| # | Əhatə dairəsinə daxil olanlar |
|---|-------------------------------|
| 1 | Dashboard səhifəsi |
| 2 | Yeni tətbiq yaratma modul səhifəsi |
| 3 | Validasiya sistemi |
| 4 | Məlumatların daxil edilməsi və təsdiqlənməsi səhifəsi |
| 5 | Təsdiq olunmuş məlumatlar səhifəsi |
| 6 | Brauzerlər arası sınaq |

## Test növləri

| # | Test növü | Təsvir |
|---|-----------|--------|
| 1 | Funksional test | Məlumatların düzgün daxil edilməsi funksionallığının yoxlanılması |
| 2 | UI testi (istifadəçi interfeysi) | Düymələrin, xanaların, yazıların yoxlanılması |
| 3 | Pozitiv test | Düzgün daxil edilmiş məlumatların idarə edilməsinin yoxlanılması |
| 4 | Reqressiya testi | Köhnə funksiyaların hazırda işlədiyinin təmin edilməsi |
| 5 | Platforma testi | Müxtəlif brauzerlərdə işlədiyinin yoxlanılması |

## Sınaq mühiti

| Element | Təfərrüatlar |
|---------|--------------|
| Əməliyyat sistemi | Windows 11 |
| Brauzerlər | Chrome, Firefox, Edge |

## Başlama meyarları

| # | Test prosesi bu şərtlər yerinə yetirildikdə başlaya bilər |
|---|-----------------------------------------------------------|
| 1 | Tələblər təsdiqlənib |
| 2 | Test məlumatları hazırlanıb |
| 3 | Smoke testlər uğurla keçirilib |

## Tamamlama meyarları

| # | Sınaq prosesi bu şərtlər yerinə yetirildikdə başa çata bilər |
|---|--------------------------------------------------------------|
| 1 | Planlaşdırılmış bütün sınaq ssenariləri icra edilib |
| 2 | Açıq vəziyyətdə heç bir Kritik və Yüksək dərəcəli nasazlıq (bug) qalmayıb |
| 3 | Uğursuz nəticələnən sınaq ssenariləri yenidən yoxlanılıb |
| 4 | Sınaq hesabatı hazırlanıb |
| 5 | Məhsul sahibi buraxılışı təsdiqləyib |

## Təhvil veriləcək nəticələr

| # | Nəticə |
|---|--------|
| 1 | Test ssenariləri |
| 2 | Nasazlıq hesabatları |
| 3 | Testin icrası hesabatı |
| 4 | Reqressiya testi hesabatı |
| 5 | QA təsdiqi |

## Test ssenariləri

| # | Title | Expected Result |
|---|-------|-----------------|
| 1 | Dashboard səhifəsini açıram | Səhifə xətasız yüklənir, bütün elementlər görünür |
| 2 | Dashboard-da "New app" düyməsinə klikləyirəm | Yeni tətbiq yaratma səhifəsi açılır |
| 3 | Yeni tətbiq yaratma səhifəsində düymələri, xanaları və yazıları yoxlayıram | Bütün xana adları, düymələr və yazılar düzgün göstərilir |
| 4 | Bütün məcburi xanaları düzgün doldururam | Məlumatlar qəbul olunur, xəta mesajı çıxmır |
| 5 | Məcburi xananı boş buraxıb göndərirəm | Xəta mesajı göstərilir, göndərmə bloklanır |
| 6 | Yanlış formatda məlumat daxil edirəm (məsələn, səhv email və ya telefon) | Uyğun validasiya mesajı göstərilir |
| 7 | Maksimum uzunluqdan artıq mətn daxil edirəm | Limit tətbiq olunur və ya xəta mesajı göstərilir |
| 8 | Xanalara xüsusi simvol və ya skript daxil edirəm | Məlumat təmizlənir və ya rədd edilir, skript icra olunmur |
| 9 | Məlumatları daxil edib təsdiq səhifəsinə keçirəm | Daxil edilmiş məlumatlar təsdiq səhifəsində düzgün göstərilir |
| 10 | Təsdiq mərhələsindən geri qayıdıram | Daxil edilmiş məlumatlar itmir |
| 11 | Məlumatları təsdiqləyirəm | Tətbiq yaradılır, məlumatlar təsdiq olunmuş siyahıda görünür |
| 12 | Təsdiq olunmuş məlumatlar səhifəsini açıram | Göstərilən məlumatlar daxil edilənlərlə üst-üstə düşür |
| 13 | Köhnə funksiyaları yoxlayıram (reqressiya) | Mövcud funksiyalar əvvəlki kimi işləyir |
| 14 | Chrome, Firefox və Edge brauzerlərində 4–12 addımlarını təkrarlayıram | Hər üç brauzerdə eyni nəticə alınır |
