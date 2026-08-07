# RFC-002: Entity

Status: Draft

## Purpose

Определить семантический примитив Entity.

## Scope

Документ описывает только семантику Entity.

## Definition

Canonical definition: DEF-003.

Entity представляет собой индивидуально адресуемый объект Semantic Model.

## Normative Requirements

EN-001 Каждая Entity имеет устойчивую адресуемость в пределах модели.

EN-002 Entity не имеет предопределённой внутренней структуры.

EN-003 Entity не определяется своим отображением.

EN-004 Entity может использоваться значением Role.

EN-005 Entity может участвовать в любом количестве Statement Instance.

## Non-goals

- идентичность;
- жизненный цикл;
- хранение;
- сериализация.

## Rationale

Entity — минимальная единица моделирования, не навязывающая способ реализации.

## References

Definitions DEF-003, DEF-010
Axioms AX-001, AX-003
