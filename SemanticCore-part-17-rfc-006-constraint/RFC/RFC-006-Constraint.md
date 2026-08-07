# RFC-006: Constraint

Status: Draft

## Purpose

Определить место Constraint в Semantic Core.

## Scope

Документ описывает только семантику Constraint.

## Definition

Canonical definition: DEF-008.

Constraint определяет дополнительное правило,
которому должны соответствовать элементы Semantic Model
в рамках конкретной Theory.

## Normative Requirements

CS-001 Constraint принадлежит Theory.

CS-002 Constraint не изменяет семантику примитивов Semantic Core.

CS-003 Constraint может ссылаться на Entity, Statement, Role и Statement Instance.

CS-004 Constraint может проверять корректность модели, но не определяет её структуру.

CS-005 Semantic Core не предписывает язык описания Constraint.

## Non-goals

- язык правил;
- механизм исполнения;
- логический вывод;
- оптимизация проверки.

## Rationale

Constraint отделяет правила конкретной предметной области от универсальной
семантической модели. Поскольку Role адресуется полным HIP, ссылка Constraint на
конкретную Role не требует отдельного механизма идентификации.

## References

DEF-008
DEF-010
AX-010
INV-006
DEC-002
DEC-015
