# RFC-003: Statement

Status: Draft

## Purpose

Определить семантический примитив Statement.

## Scope

Документ описывает только семантику Statement.

## Definition

Canonical definition: DEF-004.

Statement определяет тип семантического отношения и полный набор допустимых
Role. В базовом механизме Semantic Core семантика отношения принадлежит
Statement; конкретные Statement Instance только выражают эту семантику для
назначенных Values.

## Normative Requirements

ST-001 Statement определяет множество Role.

ST-002 Каждый Statement рассматривается как отдельное определение отношения.
Совпадение структуры двух Statement само по себе не устанавливает их
семантическую идентичность.

ST-003 Statement сам по себе не содержит значений Role.

ST-004 Значения появляются только в Statement Instance.

ST-005 Statement может иметь любое количество Role.

ST-006 Statement является единственным примитивом базового механизма Semantic
Core, который задаёт семантику отношения. Role и конкретные Value не могут
самостоятельно переопределять эту семантику.

## Non-goals

- порядок хранения;
- визуальное представление;
- ограничения Theory;
- теория семантической идентичности Statement.

## Rationale

Statement описывает форму и семантику отношения, а не конкретный факт.
Statement Instance выражает конкретный факт, применяя семантику Statement к
Values через определённые им Roles.

## References

DEF-004
AX-004
AX-005
AX-006
AX-009
AX-011
DEC-012
