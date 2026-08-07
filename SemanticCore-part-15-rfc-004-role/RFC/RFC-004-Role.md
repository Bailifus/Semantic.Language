# RFC-004: Role

Status: Draft

## Purpose

Определить семантику примитива Role.

## Scope

Документ описывает только Role.

## Definition

Canonical definitions: DEF-005 (Role), DEF-007 (Value).

Role — именованная позиция участия внутри Statement, предназначенная для
получения Value. Role определяет участие только в контексте своего Statement и
не является самостоятельным носителем семантики.

## Normative Requirements

RL-001 Role принадлежит ровно одному Statement.

RL-002 Role имеет уникальное имя в пределах Statement.

RL-003 Role не существует вне Statement.

RL-004 Каждое вхождение Role в Statement Instance имеет ровно одно значение.

RL-005 Значением Role может быть Entity, Statement либо Statement Instance.

RL-006 Role не имеет самостоятельной семантики вне Statement, которому оно
принадлежит. Имя Role идентифицирует позицию участия внутри этого Statement.

## Non-goals

- типизация значений;
- кардинальности;
- ограничения Theory.

## Rationale

Role отделяет структуру участия от конкретных Values и является точкой
связывания Statement Instance. Value может ссылаться как на объект или факт,
так и на само определение отношения. Семантика отношения задаётся Statement, а
не Role отдельно от него.

## References

DEF-005
AX-002
AX-003
DEC-003
AX-011
DEC-012
DEC-013
