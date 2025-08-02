
# 🎮 ИИ-генератор игровых квестов – GameDev AI 2025 

## 🏆 GameDev AI 25
Проект был разработан во время хакатона **"GameDev AI 25"** в рамках трека **"Генерация квестов и сюжетов"**

## Описание
Автоматическая генерация игровых RPG-квестов с помощью **Mistral AI  API**



## 👾 Stack
 - Python 3.10+
 - Mistral AI API
 - json
 - pathlib
## 👾 Ввод
.txt файл, содержащий:
 - Жанр (только RPG)
 - Главного героя
 - Цель квеста
## 👾 Вывод
JSON файл, содержащий:
 - 5-10 игровыми сценами
 - сцену с развилкой сюжета
 - основную и побочную ветви
## 👾 Принцип работы
**1. Чтение промпта и текстового файла**
- `prompt.txt` (файл с промптом для ИИ-модели)
- `plot.txt` (файл с описанием для квеста)
**2. Генерация квеста**
 - Передача данных **Mistral AI API**
 - Программа возвращает JSON объект с готовым квестом

**3. Сохранение результата**
- Создание JSON файла
- Сохранение в папку outputs

## 🚀 Запуск
### Зарегистрироваться на Mistral AI API, создать API-ключ в профиле:
https://auth.mistral.ai/ui/login?flow=2da7989e-ca6b-4cea-aa4e-ee926aa936fb

### Создать .env с переменной MISTRAL_API_KEY, в которой бует храниться ключ:
```bash
MISTRAL_API_KEY = 'ваш api-ключ'
```
### Создать виртуальное окружение и установить необходимые библиотеки:
Для Windows:
```bash
python -m venv venv
```
```bash
venv\Scripts\activate
```
```bash
pip install -r requirements.txt
```
Для MacOS:
```bash
python -m venv venv
```
```bash
source venv/bin/activate
```
```bash
pip install -r requirements.txt
```
### Запустить код

### Готово! ✨
