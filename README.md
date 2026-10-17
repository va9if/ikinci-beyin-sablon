# İkinci Beyin şablonu

AI ilə işləyəndə hər dəfə özünü yenidən tanıtmaq, layihəni yenidən izah etmək lazım olmasın deyə sadə bir sistem: Markdown fayllardan ibarət qovluq. İstənilən AI (Claude, ChatGPT, Gemini, Codex, Cursor) bu qovluğu oxuyur, sənin qaydalarını, layihələrini və qərarlarını bilir və yeni öyrəndiyini ora yazır.

Proqram, plugin və ya abunəlik lazım deyil. Yalnız Markdown və (istəsən) git.

## Necə qurulur

Üç yol var, ən asanı birincidir.

1. **Yalnız promptla.** Bu şablonu yükləmək belə lazım deyil. [vagif.co/qurulum/ikinci-beyin-promptla](https://vagif.co/qurulum/ikinci-beyin-promptla) səhifəsindəki qurucu promptu AI-a yapışdır, o qovluğu özü yaradır.
2. **GitHub şablonu.** Yuxarıdakı **Use this template** düyməsini bas, repo-nu private yarat, kompüterinə klonla. Cihazlar arasında sinxron istəyirsənsə bu yoldur. Addımlar: [vagif.co/qurulum/ikinci-beyin-github](https://vagif.co/qurulum/ikinci-beyin-github)
3. **ZIP.** Repo-nu ZIP kimi yüklə, qovluğu aç.

## İlk addım

Qovluğu AI alətində aç və yaz:

> BRAIN.md-ni oxu. Sonra mənimlə tanışlıq söhbəti apar: bir-iki sual ver, cavablarıma görə wiki/Men.md və wiki/Qaydalar.md fayllarını doldur.

## Qovluq quruluşu

```
BRAIN.md          bütün AI-ların oxuduğu qayda faylı
AGENTS.md         Codex və s. üçün BRAIN.md-yə yönləndirmə
CLAUDE.md         Claude üçün BRAIN.md-yə yönləndirmə
GEMINI.md         Gemini üçün BRAIN.md-yə yönləndirmə
wiki/             təmiz, bir-birinə bağlı səhifələr
  Men.md          sən kimsən, necə işləyirsən
  Qaydalar.md     AI-a verdiyin davamlı göstərişlər
  Layiheler.md    layihə indeksi
  Qerarlar.md     qərar indeksi
  Insanlar.md     müştəri və tərəfdaş indeksi
  layiheler/      hər layihə üçün bir səhifə
  insanlar/       hər insan üçün bir səhifə
raw/              xam qeydlər
  qerarlar/       hər vacib qərarın tam izahı
  qeydler/        faydalı söhbət nəticələri
sablonlar/        yeni səhifələr üçün şablonlar
```

`raw/` xam material, `wiki/` isə ondan çıxarılmış sadə və linklənmiş xülasədir. AI əvvəl `wiki/` oxuyur, lazım olsa `raw/`-a düşür.

## Obsidian (istəyə görə)

Qovluğu [Obsidian](https://obsidian.md)-də "vault" kimi aç. `[[vikilink]]`-lər və qraf görünüşü işləyəcək. Sistemin işləməsi üçün Obsidian lazım deyil.

## Təhlükəsizlik

- Parol, token, API açarı, kart və sənəd nömrəsi bura yazılmır. `BRAIN.md` AI-a bunu qadağan edir, amma son nəzarət səndədir.
- GitHub-a göndərirsənsə repo-nu **private** saxla.
- AI-ın yazdığı hər şeyi vaxtaşırı oxu. Yanlış fakt görsən düzəlt, çünki AI növbəti dəfə ona güvənəcək.

## Mənbə

Bu sistem Andrej Karpathy-nin raw/wiki yanaşmasına əsaslanır və gündəlik iş üçün sadələşdirilib. Hazırlayan: [Vagif Ibrahimov](https://vagif.co). MIT lisenziyası: istədiyin kimi istifadə et, dəyiş, paylaş.
