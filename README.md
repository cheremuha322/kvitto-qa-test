# Тестовое задание Junior QA Engineer — Квитто

**Выполнил:** Колесников Владислав  
**Стенд:** https://kvitto-qa-demo.vercel.app  
**Дата:** 06.10.2026

## Артефакты тестирования

### Google Таблица
https://docs.google.com/spreadsheets/d/1rwkXzzBmhgCLwuTCgDHM1F4BBWib4PpK7Mtgtqev_3U/edit?usp=sharing

Содержит три листа:
- **Тест-кейсы** — 9 сценариев проверки UI (позитивные, негативные, граничные значения)
- **Баги** — все найденные дефекты интерфейса и API с подробным описанием
- **Итог** — заключение для Product Manager

### Postman
В папке `/postman` находятся:
- `Kvitto_Collection.json` — коллекция из 6 запросов с автоматическими проверками (pm.test)
- `Kvitto_Env.json` — окружение с переменными base_url и payment_id

##  Бонус: Автотесты API

В папке `/auto_tests` реализованы автотесты на Python (pytest + requests), проверяющие базовые сценарии API.

### Запуск тестов

```bash
# Клонировать репозиторий
git clone https://github.com/ВАШ_НИК/kvitto-qa-test.git
cd kvitto-qa-test

# Установить зависимости
pip install -r auto_tests/requirements.txt

# Запустить тесты
pytest auto_tests/test_api.py -v
