# Chaos Engineering Manual

## Introduction

We document a chaos engineering process the way it works 
in industrial-grade practice. It's not magic, it's just 
plenty of things to care about and decide on.

## Who can use this manual?

- highload projects (cost implementation)
- actively maintained (detecting a detecting vulnerability without fixing will not help)
- distributed systems (fewer things break in a monolith)
- mature mindset for reliability (attach value and willing to allocate resources for system reliability)

## Process // Как мы работаем

The manual describes a chaos engineering process starting 
from incident categorization and system research to 
hypothesis/well functioning tests. The process outcomes are team tasks 
for fixing failed tests and suites of green tests (to be invoked on new release).

### Подготовка:

- начинаем с анализа истории инцидентов
- сводим к категориям инцидентов (grow up)
- делаем исследование (что на входе, что не выходе)
- строим гипотезы и планируем эксперименты в местах "где узко"
- используем группы атак (в том числе по сложности и стоимости подготовки тестов)

### Тестирование:

- провели тесты, зафиксирвоали результаты
- получили в несколько итераций эталонные тесты 

### Что делаем с результатами:

- что считаем положительным или отрицательным результатом теста

Отрицательные тесты:

- задача на исследование команде (почему так получилось)
- распочковывание задач команде + проблемы + риски

Тесты, которые проходят:

- используем для анализа следующего релиза
- при необходимости - проводим на их основе аварийные учения

## Types of incidents

The standard list of incidents can be [found here](https://www.gremlin.com/docs/infrastructure-layer/attacks/)

We follow a slightly different grouping that enables us to prioritize complexity and costs of staging the tests.


## FAQ

- What software should I use?
- How do we sell chaos engineering inside our organisation?
- Does chaos engineering help for smaller systems?

## Glossary

- chaos engineeering 
- attack
- incident

## Feedback 

Please leave a note or question in [Github issues](https://github.com/epogrebnyak/chaos-manual/issues).

You can also follow us [on Twitter](https://twitter.com/v10n10).
