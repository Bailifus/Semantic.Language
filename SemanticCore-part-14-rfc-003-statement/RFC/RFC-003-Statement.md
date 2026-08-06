# RFC-003: Statement

Status: Draft

## Purpose

Определить семантический примитив Statement.

## Scope

Документ описывает только семантику Statement.

## Definition

Canonical definition: DEF-004.

Statement определяет тип отношения и полный набор допустимых Role.

## Normative Requirements

ST-001 Statement определяет множество Role.

ST-002 Каждый Statement имеет собственную идентичность как определение отношения.

ST-003 Statement сам по себе не содержит значений Role.

ST-004 Значения появляются только в Statement Instance.

ST-005 Statement может иметь любое количество Role.

## Non-goals

- порядок хранения;
- визуальное представление;
- ограничения Theory.

## Rationale

Statement описывает форму отношения, а не конкретный факт.

## References

DEF-004
AX-004
AX-005
