# RFC-015: Semantic Zoom

Status: Draft

## Purpose

Определить требования к механизму Semantic Zoom.

## Scope

Документ описывает только изменение представления модели при масштабировании.

## Definition

Semantic Zoom — механизм изменения Presentation в зависимости от уровня
масштабирования без изменения Semantic Model.

## Normative Requirements

SZ-001 Semantic Zoom влияет только на Presentation.

SZ-002 Semantic Zoom не изменяет Semantic Model.

SZ-003 При изменении масштаба допускается скрытие и отображение элементов,
но не изменение их семантики.

SZ-004 Любой элемент, скрытый на одном масштабе, должен быть доступен
на подходящем уровне масштабирования.

SZ-005 Semantic Zoom должен быть совместим с Level of Detail.

## Non-goals

- алгоритмы размещения;
- анимация;
- пользовательский интерфейс;
- конкретные графические библиотеки.

## Rationale

Semantic Zoom позволяет создавать удобные интерактивные представления,
не нарушая семантическую целостность модели.

## References

RFC-013 Presentation Model
RFC-014 Level of Detail
INV-001
INV-003
INV-004
