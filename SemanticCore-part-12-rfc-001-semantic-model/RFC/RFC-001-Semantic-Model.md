# RFC-001: Semantic Model

Status: Draft

## Purpose

Определить фундаментальную структуру Semantic Model.

## Scope

Документ описывает только семантическую модель.
Хранение, API, сериализация и представление не рассматриваются.

## Normative Requirements

SM-001 Semantic Model состоит исключительно из семантических примитивов.

SM-002 Semantic Model не зависит от способа хранения.

SM-003 Semantic Model не зависит от способа отображения.

SM-004 Semantic Model не зависит от конкретной Theory.

SM-005 Все нормативные конструкции модели выражаются через примитивы Semantic Core.

## Non-goals

- UI
- Базы данных
- API
- Оптимизация
- Форматы файлов

## Rationale

Разделение модели и реализации позволяет создавать независимые совместимые реализации.

## References

RFC-000 Constitution
Definitions
Axioms
Invariants
