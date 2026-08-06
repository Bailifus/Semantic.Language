# RFC-004: Role

Status: Draft

## Purpose

Определить семантику примитива Role.

## Scope

Документ описывает только Role.

## Definition

Canonical definitions: DEF-005 (Role), DEF-007 (Value).

Role — именованная позиция внутри Statement, предназначенная для получения значения.

## Normative Requirements

RL-001 Role принадлежит ровно одному Statement.

RL-002 Role имеет уникальное имя в пределах Statement.

RL-003 Role не существует вне Statement.

RL-004 Каждое вхождение Role в Statement Instance имеет ровно одно значение.

RL-005 Значением Role может быть Entity либо Statement Instance.

## Non-goals

- типизация значений;
- кардинальности;
- ограничения Theory.

## Rationale

Role отделяет структуру отношения от конкретных значений и является точкой связывания модели.

## References

DEF-005
AX-002
AX-003
DEC-003
