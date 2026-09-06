# Persefoni Connector — Connector Discovery

**Category:** C48. Environmental, Social & Governance (ESG) Reporting  
**Vendor:** Persefoni  
**Official Website:** https://www.persefoni.com

## 1. Официальный API
- **Базовый URL API:** `https://api.persefoni.com/v1`
- **Поддерживаемая модель авторизации:** OAuth 2.0 Client Credentials Grant

## 2. Архитектура сущностей
- Ключевые ресурсы платформы Persefoni:
  - учетные транзакции (/activities)
  - расчетные углеродные эквиваленты (/footprints)
  - портфельные компании
  - аудиторские срезы

## 3. Требования к отказоустойчивости и безопасности
- Соблюдение вендорных лимитов запросов (Rate Limiting) с экспоненциальной задержкой.
- Строгая валидация Pydantic-схем на входе и выходе каждого запроса.
- Тестовая точка проверки подключения: `GET /v1/organizations`.
