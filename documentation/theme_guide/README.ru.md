📘 This documentation is also available in [English](README.md)

---

## 📋 Содержание
- [Обзор](#обзор)
- [Создание папки темы](#создание-папки-темы)
- [Файл стилей](#файл-стилей)
- [Метаинформация](#метаинформация)
- [Скриншоты](#скриншоты)
- [Шрифты и иконки](#шрифты-и-иконки)

---

## 📖 Обзор

Темы в `PortProtonQT` позволяют изменить внешний вид интерфейса. Все темы хранятся в папке:

- `~/.local/share/PortProtonQT/themes`.

---

## 📁 Создание папки темы

```bash
mkdir -p ~/.local/share/PortProtonQT/themes/my_custom_theme
```

---

## 🎨 Файл стилей (`styles.py`)

Создайте `styles.py` в корне темы. В нём определите переменные и/или функции, возвращающие CSS-оформление.

**Пример функции:**
```python
def custom_button_style(color1, color2):
    return f"""
    QPushButton {{
        background: qlineargradient(x1:0, y1:0, x2:1, y2:0,
                                    stop:0 {color1}, stop:1 {color2});
    }}
    """
```

---

## 📝 Метаинформация (`metainfo.ini`)

```ini
[Metainfo]
name = My Custom Theme
author = Ваше имя
author_link = https://example.com
description = Описание вашей темы.
```

---

## 🖼 Скриншоты

Папка: `images/screenshots/` — любые изображения оформления темы.

---

## 🔡 Шрифты и иконки (опционально)

- Шрифты: `fonts/*.ttf` или `.otf`
- Иконки: `images/icons/*.svg/.png`

---
