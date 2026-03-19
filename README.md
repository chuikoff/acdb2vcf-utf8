# acdb2vcf-utf8 (улучшенный форк)

**Быстрый и качественный конвертер contacts2.db → VCF 3.0** с исправлением Unicode (эмодзи, русские буквы) для Windows.

Оригинальный проект: [RuslanUC/acdb2vcf](https://github.com/RuslanUC/acdb2vcf)  
Спасибо автору **RuslanUC**!

## Что исправлено
- Полная поддержка UTF-8 (эмодзи 🐊, русские имена, WhatsApp и т.д.)
- Работает на Python 3.11+ без ошибок `charmap codec`
- Улучшенный русский README
- Полная поддержка UTF-8 (эмодзи, русские имена)
- Поддержка фото аватаров (BLOB → base64 PHOTO;TYPE=JPEG/PNG)

## Установка и использование

```powershell
# 1. Скачай этот репозиторий или просто acdb2vcf.py
git clone https://github.com/ТВОЙ_НИК/acdb2vcf-utf8.git

# 2. Положи contacts2.db рядом

# 3. Посмотреть аккаунты
python3 acdb2vcf.py --list-accounts contacts2.db

# 4. Конвертировать всё
python3 acdb2vcf.py --all contacts2.db my_contacts.vcf


