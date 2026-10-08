# Markdown denetim aracı: markdownlint-cli2

Date: 2026-10-08

Markdown dosyalarını denetlemek için markdownlint-cli2 seçildi. Gerekçe: tek bir yapılandırma dosyasıyla (`.markdownlint-cli2.yaml`) çalışıyor, Node dışında bağımlılık istemiyor ve GitHub Actions ile kolay kullanılıyor. Reddedilen seçenek: remark-lint; daha esnek ama bu küçük depo için fazla. Yapılandırma: varsayılan kurallar açık, MD013 (satır uzunluğu) kapalı, çünkü README'de uzun düzyazı satırları var. `.ai/**`, `AGENTS.md` ve `CLAUDE.md` Coditor/Context Bank'ın ürettiği bağlam dosyaları olduğu için denetim dışında.
