# RFC-007: Theory

Status: Draft

## Purpose

Определить роль Theory как механизма расширения Semantic Core.

## Scope

Документ описывает только семантику Theory.

## Definition

Canonical definition: DEF-001.

Theory представляет собой согласованный набор семантических правил,
определений и Constraint, расширяющих Semantic Core без изменения его
базовой семантики.

## Normative Requirements

TH-001 Theory может определять собственные Constraint.

TH-002 Theory может вводить дополнительные понятия, не изменяя примитивы Semantic Core.

TH-003 Несколько Theory могут использовать одну и ту же Semantic Model.

TH-004 Semantic Core не требует наличия конкретной Theory.

TH-005 Theory должна быть явно идентифицируема.

## Non-goals

- язык описания Theory;
- механизм вывода;
- управление версиями;
- импорт и композиция Theory.

## Rationale

Theory изолирует предметную семантику от универсального ядра и позволяет
независимо развивать специализированные модели.

## References

DEF-001
INV-006
DEC-002
RFC-006 Constraint
