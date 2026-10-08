# Katkı Rehberi

Bu depo, bir Coditor bot incelemesinin GitHub dal koruması zorunlu onaylarına
sayılıp sayılmadığını test etmek için var olan atılabilir bir test deposudur.
Aşağıdaki kararlar bu küçük kapsamı yansıtır.

## Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır (telif: 2026 devtechnogit).

- **Neden MIT:** Deponun amacı herkesin bu depoyu serbestçe kopyalayıp
  denemesi. MIT en kısa ve en yaygın izin veren lisans.
- **Reddedilen alternatif:** Apache-2.0. Patent maddesi bu küçük test
  deposu için gereksiz bulundu.

## Markdown denetimi

Markdown dosyaları markdownlint-cli2 ile denetlenir.

- **Neden markdownlint-cli2:** Tek bir yapılandırma dosyasıyla
  (`.markdownlint-cli2.yaml`) çalışıyor, Node dışında bağımlılık istemiyor
  ve GitHub Actions ile kolay kullanılıyor.
- **Reddedilen alternatif:** remark-lint. Daha esnek ama bu küçük depo
  için fazla.
- **Yapılandırma:** Varsayılan kurallar açık, MD013 (satır uzunluğu)
  kapalı çünkü README'de uzun düzyazı satırları var. `.ai/**`,
  `AGENTS.md` ve `CLAUDE.md` Coditor/Context Bank'ın ürettiği bağlam
  dosyaları olduğu için denetim dışında.
- **Yerelde çalıştırma:** `npx markdownlint-cli2`. Henüz bir
  `package.json` veya bu komutu çalıştıran bir CI adımı yok.

## Katkı akışı

- Değişiklikler yalnızca taslak (draft) pull request ile `main` dalına
  girer; `main` dalına doğrudan push yapılmaz.
- Commit mesajları [Conventional Commits](https://www.conventionalcommits.org/)
  biçimindedir, örn. `feat:`, `fix:`, `docs:`, `test:`, `chore(scope):`.
