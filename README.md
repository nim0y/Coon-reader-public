<p align="center">
  <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/android/android.png" alt="Android Logo" width="100"/>
</p>

<h1 align="center">Coon Reader (Reader-pet) 🦝📚</h1>

<p align="center">
  Современное, легкое и быстрое Android-приложение для чтения электронных книг, разработанное с использованием Jetpack Compose и принципов Clean Architecture.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Kotlin-1.9.0+-blue.svg?logo=kotlin" alt="Kotlin">
  <img src="https://img.shields.io/badge/Jetpack_Compose-Material_3-4CAF50.svg?logo=android" alt="Jetpack Compose">
  <img src="https://img.shields.io/badge/Architecture-Clean_Architecture-orange.svg" alt="Clean Architecture">
</p>

---

## 📱 Скриншоты

<p align="center">
  <img src=screenshots/Screenshot_2026-03-27-17-48-18-123_com.example.coon_reader.jpg width="24%">
  <img src=screenshots/Screenshot_2026-03-27-17-48-31-556_com.example.coon_reader.jpg width="24%">
  <img src=screenshots/Screenshot_2026-03-27-17-48-50-221_com.example.coon_reader.jpg width="24%">
  <img src=screenshots/Screenshot_2026-03-27-17-48-55-532_com.example.coon_reader.jpg width="24%">
  <img src=screenshots/Screenshot_2026-03-27-17-49-12-318_com.example.coon_reader.jpg width="24%">
</p>

---

## ✨ Основные возможности

### 📖 Чтение без границ
* **Поддержка форматов:** `FB2` (включая `.zip`), `EPUB`, `PDF`, `MOBI`, `AZW3`.
* **Два режима парсинга:**
    * 🚀 *Обычный:* быстрая загрузка всей книги в память.
    * 🌊 *Потоковый (Streaming):* чтение файлов по частям (идеально для огромных книг и экономии оперативной памяти).
* **Навигация:** Удобное оглавление, поддержка сносок (примечаний) прямо внутри текста.
* **Прогресс:** Автоматическое сохранение позиции чтения для каждой книги.

### 🔍 Поиск и открытия
* **Интеграция с Google Books:** Ищите книги в огромной онлайн-библиотеке прямо из приложения.
* **Детальная информация:** Просмотр описаний, авторов, издателей и категорий.
* **Онлайн-предпросмотр:** Возможность просмотреть фрагмент книги через встроенный WebView.

### 🎨 Персонализация
* **Темы:** Поддержка светлой и темной тем (с автоматическим переключением).
* **Типографика:** Настройка размера шрифта «на лету» во время чтения.
* **Material 3:** Современный дизайн с использованием динамических цветов (Android 12+).

---

## 🛠 Технологический стек

Проект построен на самых современных решениях в мире Android-разработки:

* **Язык:** Kotlin
* **UI:** Jetpack Compose (полностью декларативный интерфейс)
* **Архитектура:** Clean Architecture + MVVM + MVI-подобный стейт
* **Инъекция зависимостей:** Dagger Hilt
* **Локальное хранилище:** Room (база данных книг и прогресса) + DataStore Preferences (настройки)
* **Сеть:** Retrofit 2 + OkHttp + Gson (взаимодействие с API Google Books)
* **Изображения:** Coil (асинхронная загрузка обложек)
* **Асинхронность:** Kotlin Coroutines & Flow
* **Аналитика:** Firebase Analytics (вынесена в независимый модуль)

---

## 📂 Структура проекта

Проект использует многомодульную архитектуру для лучшей масштабируемости и изоляции кода:

```text
📦 CoonReader
 ┣ 📂 app                  # Основной модуль Android-приложения
 ┃ ┣ 📂 data               # Репозитории, БД (Room), парсеры (FB2/EPUB/PDF), API
 ┃ ┣ 📂 domain             # Бизнес-логика, UseCases (интеракторы), модели, интерфейсы
 ┃ ┣ 📂 di                 # Модули Dagger Hilt
 ┃ ┗ 📂 ui                 # Compose-экраны, ViewModels, Темы, Диалоги
 ┗ 📂 firebase-module      # Изолированный модуль аналитики (AnalyticsManager)
```
##🚀 Как собрать и запустить

Выкладываю на RuStore ...

---

## 📈 Аналитика

Приложение использует кастомную и безопасную систему аналитики (без сбора персональных данных) для улучшения пользовательского опыта. Отслеживается:

* Успешность импорта различных форматов файлов.
* Ошибки парсинга (для оперативного исправления багов).
* Предпочтения пользователей в выборе режима чтения (Streaming vs Normal).
* Использование поисковых запросов и фильтрации жанров.

---
<p align="center">
<b>Coon Reader</b> — Сделано с ❤️ к чтению и чистому коду. 🐾📖
</p>
