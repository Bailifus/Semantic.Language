# RFC-014: Level of Detail

Status: Draft

## Purpose
Определить нормативные требования к Level of Detail.

## Scope
Документ описывает только LOD.

## Definition
Level of Detail (LOD) определяет объём информации, отображаемой Presentation, без изменения Semantic Model.

## Normative Requirements

LOD-001 LOD влияет только на Presentation.
LOD-002 Изменение LOD не должно изменять Semantic Model.
LOD-003 Скрытые элементы должны оставаться доступными на другом уровне детализации.
LOD-004 Несколько Presentation могут использовать различные LOD для одной Semantic Model.
LOD-005 Переход между уровнями детализации не должен приводить к потере семантики.

## Non-goals

- алгоритмы масштабирования;
- UI;
- компоновка.

## References

RFC-013 Presentation Model
INV-001
INV-003
INV-004
