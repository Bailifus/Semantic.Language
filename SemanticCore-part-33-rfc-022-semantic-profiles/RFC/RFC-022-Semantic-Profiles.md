# RFC-022: Semantic Profiles

Status: Draft

## Purpose

Определить механизм формирования профилей Semantic Core.

## Scope

Документ определяет требования к профилям совместимости.

## Definition

Semantic Profile — формально определённое подмножество требований
Semantic Core, предназначенное для конкретного класса реализаций.

## Normative Requirements

SP-001 Каждый профиль должен иметь уникальное имя.

SP-002 Каждый профиль должен явно перечислять включённые RFC и требования.

SP-003 Реализация должна явно указывать поддерживаемые профили.

SP-004 Профиль не может изменять смысл нормативных требований RFC.

SP-005 Реализация нескольких профилей должна сохранять взаимную совместимость
в общей области требований.

## Suggested Profiles

- Core Profile
- Visualization Profile
- Exchange Profile
- Reasoning Profile

## Non-goals

- механизм установки профилей;
- лицензирование;
- управление зависимостями.

## Rationale

Профили позволяют различным системам реализовывать только необходимую
часть стандарта, сохраняя совместимость.

## References

RFC-011 Conformance
RFC-019 Interoperability
RFC-020 Compliance Levels
RFC-021 Conformance Test Suite
