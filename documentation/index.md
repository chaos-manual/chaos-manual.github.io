# Chaos Engineering Manual

We document a chaos engineering process the way it works in practice. 
It's no magic, it's plenty of things to care about.

## Project review

The manual describes a working chaos engineering process starting 
from incident categorization and system research to 
hypothesis/well functioning tests. The process outcomes are team tasks 
for fixing failed tests and suites of green tests (to be invoked on new release).

We follow a slightly different grouping of incident types that enables us 
to prioritize complexity and costs of staging the tests.

## Как мы работаем

- начинаем с анализа истории инцидентов
- сводим к категориям инцидентов (grow up)
- делаем исследование
- строим гипотезы и планируем эксперименты в местах "где узко"
- группы атак (в том числе по сложности подготовки тестов) - это понятие 
- провели тесты 
- получили в несколько итераций эталонные тесты 
- задача на исследование команде (почему так получилось)
- распочковывание задач команде + проблемы + риски
- тесты, которые проходят