---
title: "Büyük Metin Verilerinde Tanımlayıcı Bilgilerin Hesaplamalı Yöntemlerle Anonimleştirilmesi"
date: 2026-02-15
summary: "Metin veri setlerindeki hassas bilgilerin anonimleştirilmesine yönelik hesaplamalı tekniklerin incelenmesi."
tags: ["data privacy", "NLP", "text analysis"]
featured_image: "featured.png"

organization: "Pew Research Center"
tools: ["R", "Python", "NLP libraries", "Hugging Face", "transformers"]

external_link: "https://www.pewresearch.org/decoded/2024/01/12/redacting-identifying-information-with-computational-methods-in-large-text-data/"
link_text: "Blog yazısını oku →"

work_group: "public-opinion"
---
Bu blog yazısı, araştırmacıların yapılandırılmamış metin verilerinden — ABD K-12 okul bölgelerine ait 1.314 misyon ifadesinden oluşan bir veri setinden — tanımlayıcı bilgileri, kamuya açık yayından önce hesaplamalı yöntemlerle nasıl temizlediğini açıklamaktadır. Yapılandırılmış veri setlerinde bölge adları gibi tanımlayıcıları kaldırmak görece kolaydır; ancak serbest biçimli metinlerde isimler veya adresler için sabit etiketler olmadığından bu işlem çok daha güçtür. Bu sorunu çözmek için araştırmacılar üç farklı tekniği bir arada kullandı:

- Bilinen bölge adlarının harici bir listeyle tam eşleştirilmesi,
- Kuruluş adlarını tespit etmek için önceden eğitilmiş modellerle Adlandırılmış Varlık Tanıma (NER), ve
- "Okul" veya "bölge" kelimelerinden önce gelen büyük harfli sözcük kalıplarını tespit etmek için düzenli ifadeler.

Her yaklaşımın tek başına sınırlılıkları bulunduğundan, doğru anonimleştirilen terimleri en üst düzeye çıkarırken hatalı pozitif sonuçları en aza indirmek amacıyla bu teknikler birlikte kullanıldı.

## Katkım

Büyük metin korpuslarından kişisel tanımlayıcı bilgileri tespit etmek ve kaldırmak için ölçeklenebilir NLP yaklaşımları geliştirdim ve değerlendirdim; bu yöntemlerin araştırma şeffaflığı ve veri gizliliği açısından sonuçlarını kamuya yönelik bir blog yazısında aktardım.
