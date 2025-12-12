# 🕵️ Spy Game Words Dataset

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

**[English]**  
This repository hosts the community-driven database of words for the "Spy" party game. The file `ru.json` is the main source of content. You can easily contribute by adding new words, categories, or fixing errors.

**[Русский]**  
В этом репозитории хранится база слов для игры «Шпион», которую мы собираем всем сообществом. Файл `ru.json` — это основной источник контента. Вы можете легко помочь проекту, добавив новые слова, категории или исправив ошибки.

---

## 🌍 How to Contribute / Как добавить слова

### 1. The Easy Way (Простой способ)
If you don't know how to use Git:
1. Go to the **[Issues](https://github.com/YOUR_USERNAME/REPO_NAME/issues)** tab.
2. Click **New Issue**.
3. Write the words you want to add (and their category).
4. We will add them for you!

**На русском:**
Если вы не умеете программировать:
1. Перейдите во вкладку **[Issues](https://github.com/YOUR_USERNAME/REPO_NAME/issues)** (Задачи).
2. Нажмите **New Issue** (Новая задача).
3. Просто напишите список слов и категорию, в которую их нужно добавить.
4. Мы добавим их в файл сами!

### 2. The Developer Way (Через Pull Request)
1. Fork this repository.
2. Edit `ru.json`.
3. Create a Pull Request.

---

## 📂 Data Structure / Структура данных

The file uses strict JSON format. Please validate your JSON before submitting (use [jsonlint.com](https://jsonlint.com)).

Файл использует строгий формат JSON. Пожалуйста, проверяйте валидность кода перед отправкой (например, на [jsonlint.com](https://jsonlint.com)).

### Word Object / Объект слова
Every word must have a `text` and a `type`. Optionally, it can be marked as `isAdult`.

Каждое слово должно иметь `text` и `type`. Опционально можно добавить флаг `isAdult` (18+).

```json
{
  "text": "Bank",           // The word itself / Слово
  "type": "location",       // Type (see below) / Тип (см. ниже)
  "isAdult": true           // Optional: Only for 18+ content / Только для контента 18+
}
