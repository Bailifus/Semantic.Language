# RFC-013: Presentation Model

Status: Draft

## Purpose

Определить правила представления Semantic Model без изменения её семантики.

## Scope

Документ описывает требования к Presentation.

## Definition

Presentation — произвольное визуальное или текстовое отображение Semantic Model,
предназначенное для человека или программного средства.

## Normative Requirements

PR-001 Presentation не должна изменять семантику модели.

PR-002 Один Presentation может отображать только часть Semantic Model.

PR-003 Одна Semantic Model может иметь множество различных Presentation.

PR-004 Presentation может использовать Level of Detail для скрытия информации.

PR-005 Скрытие информации не должно приводить к её утрате.

PR-006 Canonical Diagram является производным Presentation Canonical Text и не
может использоваться для изменения или переопределения нормативной семантики.

## Non-goals

- пользовательский интерфейс;
- графический стиль;
- редакторы;
- интерактивное поведение.

## Rationale

Presentation отделяет способ восприятия модели от самой модели,
сохраняя возможность создания специализированных представлений.

## References

RFC-001 Semantic Model
RFC-009 Canonical Text
RFC-010 Canonical Diagram
INV-001
INV-003
