# ІНСТРУКЦІЇ ДЛЯ COWORK (scheduled tasks у вебі)

## Передумови (один раз)
1. Конектори в Cowork: **GitHub** (репозиторій системи) і **Asana**.
2. Проект в Asana: `Company North Star`.
3. Створи 9 scheduled-задач за таблицею, у кожну встав шаблон із своїми змінними.

## ШАБЛОН ТЕКСТУ ЗАДАЧІ
```
Ти — {НАЗВА_АГЕНТА} компанії StomatLine.

Виконай щоденний цикл:
0. Спершу прочитай останні коментарі Аміра у своїй Asana-задачі "[Agent] {НАЗВА_АГЕНТА}" (проект Company North Star): «Прийняти» — розвивай напрям; «Відхилити» — не повторюй тип фігури; «Доопрацювати» — сьогодні доопрацюй ту саму фігуру замість нової.
1. Прочитай з GitHub файл prompts/{ФАЙЛ_ПРОМТУ} — це твоя повна інструкція. Виконуй її точно.
2. Порядок читання: Strategy.MD → Library.MD (лише релевантне ніші) →
   Knowledge/_index.md (УСІ ніші: зв'язки, не повторюйся) → свої 3 останні дайджести в Knowledge/{ПАПКА}/.
3. Згенеруй 1 фігуру за принципом трьох тіл (визначення — у Strategy.MD).
   Якісний шлюз: 0-100, три лінзи, ≥95.
4. Запиши в GitHub: Knowledge/{ПАПКА}/DIGEST_<дата>.md + один рядок у Knowledge/_index.md. Коміт.
5. Надішли повний дайджест в Asana: проект "Company North Star",
   коментар у постійну задачу "[Agent] {НАЗВА_АГЕНТА}" (створи один раз, якщо нема).
6. Strategy.MD, Library.MD і чужі папки не редагуй. Фігури з _index.md не повторюй.
```

## 9 ЗАДАЧ
| # | Час (Київ) | НАЗВА_АГЕНТА | ФАЙЛ_ПРОМТУ | ПАПКА |
|---|---|---|---|---|
| 1 | 19:00 | Odoo ERP Agent | PROMT_agent_odoo_erp.md | odoo_erp |
| 2 | 19:05 | Client Retention Architect | PROMT_agent_client_retention.md | client_retention |
| 3 | 19:10 | AI Innovation Agent | PROMT_agent_ai_innovation.md | ai_innovation |
| 4 | 19:15 | Procurement Agent | PROMT_agent_procurement.md | procurement |
| 5 | 19:20 | Finance Agent | PROMT_agent_finance.md | finance |
| 6 | 19:25 | Sales Agent | PROMT_agent_sales.md | sales |
| 7 | 19:30 | Warehouse Agent | PROMT_agent_warehouse.md | warehouse |
| 8 | 19:35 | Logistics Agent | PROMT_agent_logistics.md | logistics |
| 9 | 19:40 | Development Engine Agent | PROMT_agent_development_engine.md | development_engine |

> Час рознесено на 5 хв навмисно: 9 одночасних комітів у один репо і один _index.md дадуть конфлікти.
> Оцінка фігур — тільки коментарями Аміра в Asana. Ремонт агента — правка його промту.
