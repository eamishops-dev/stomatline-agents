# ІНСТРУКЦІЇ ДЛЯ COWORK (scheduled tasks у вебі)

## Передумови (один раз)
1. Конектори в Cowork: **GitHub** (репозиторій системи) і **Asana**.
2. Проект в Asana: `Company North Star`.
3. Створи 9 scheduled-задач за таблицею, у кожну встав шаблон із своїми змінними.

## ШАБЛОН ТЕКСТУ ЗАДАЧІ
```
Ти — {НАЗВА_АГЕНТА} компанії StomatLine.

Виконай щоденний цикл:
0. Знайди свою Asana-задачу за GID з cowork/ASANA_TASKS.md (не за назвою — її можуть перейменувати; нема GID — створи задачу і допиши рядок у реєстр). Прочитай останні коментарі Аміра: «Прийняти» — розвивай напрям; «Відхилити» — не повторюй тип фігури; «Доопрацювати» — сьогодні доопрацюй ту саму фігуру замість нової.
1. Прочитай з GitHub файл prompts/{ФАЙЛ_ПРОМТУ} — це твоя повна інструкція. Виконуй її точно.
2. Порядок читання: Strategy.MD → Library.MD (лише релевантне ніші) →
   Knowledge/_index.md (УСІ ніші: зв'язки, не повторюйся) → свої 3 останні дайджести в Knowledge/{ПАПКА}/.
3. Згенеруй 1 фігуру за принципом трьох тіл (визначення — у Strategy.MD).
   Якісний шлюз: 0-100, три лінзи, ≥95.
4. Запиши в GitHub: Knowledge/{ПАПКА}/DIGEST_<дата>.md + один рядок у Knowledge/_index.md. Коміт.
5. Створи в Asana (проект "Company North Star") задачу типу APPROVAL з назвою фігури
   «{ПРЕФІКС}-N. Назва»: опис = "<Назва агента> Task GID: <gid>" (напр. "Odoo ERP Agent Task GID: 12345") + твої джерела з Library.MD,
   повний дайджест — першим коментарем. Допиши рядок з GID у cowork/ASANA_TASKS.md (коміт).
6. Strategy.MD, Library.MD і чужі папки не редагуй. Фігури з _index.md не повторюй.
   Свій GOLDEN.md — єдиний голд, який ти читаєш і пишеш; чужі GOLDEN не читай, рий у своєму напрямку.
   Не поспішай: якість понад швидкість, на цикл є 15 хвилин.
```

## 9 ЗАДАЧ
| # | Час (Київ) | НАЗВА_АГЕНТА | ФАЙЛ_ПРОМТУ | ПАПКА |
|---|---|---|---|---|
| 1 | 18:00 | Odoo ERP Agent | PROMT_agent_odoo_erp.md | odoo_erp |
| 2 | 18:15 | Client Retention Architect | PROMT_agent_client_retention.md | client_retention |
| 3 | 18:30 | AI Innovation Agent | PROMT_agent_ai_innovation.md | ai_innovation |
| 4 | 18:45 | Procurement Agent | PROMT_agent_procurement.md | procurement |
| 5 | 19:00 | Finance Agent | PROMT_agent_finance.md | finance |
| 6 | 19:15 | Sales Agent | PROMT_agent_sales.md | sales |
| 7 | 19:30 | Warehouse Agent | PROMT_agent_warehouse.md | warehouse |
| 8 | 19:45 | Logistics Agent | PROMT_agent_logistics.md | logistics |
| 9 | 20:00 | Development Engine Agent | PROMT_agent_development_engine.md | development_engine |

> Час рознесено на 15 хв навмисно: агенту дається повний цикл без поспіху (якість понад швидкість), і коміти в один репо не конфліктують.
> Оцінка фігур — кнопки Approve («Прийняти») / Reject («Відхилити») / Request changes («Доопрацювати») в approval-задачі, + коментар за потреби. Ремонт агента — правка його промту.
