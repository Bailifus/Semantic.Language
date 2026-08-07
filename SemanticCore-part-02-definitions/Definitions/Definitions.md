# Definitions

## Role of this document

This document is the canonical machine-oriented registry of Semantic Core terms.
Each normative term has one stable identifier and one compact definition here.

RFC documents provide human-oriented explanation, rationale, and normative
requirements. A defining RFC must reference the corresponding `DEF-xxx`
identifier, and the registry must reference the defining RFC where one exists.

If documents appear to conflict:

1. `Definitions.md` controls the identity and compact core meaning of a term;
2. the relevant RFC controls its detailed normative behaviour;
3. the Glossary is navigational and has no independent definitional authority;
4. an actual contradiction between the registry and an RFC is a specification
   defect and must be corrected rather than interpreted as an override.

## DEF-001 Theory
Набор семантических правил, ограничений и интерпретаций.

Human-readable specification: RFC-007.

## DEF-002 Domain
Область моделирования, внутри которой определены сущности и утверждения.

## DEF-003 Entity
Индивидуально адресуемый (DEF-010) объект модели.

Human-readable specification: RFC-002.

## DEF-004 Statement
Индивидуально адресуемое (DEF-010) определение типа семантического отношения,
задающее полный набор Role.

В базовом механизме Semantic Core Statement является единственным примитивом,
который задаёт семантику отношения. Конкретный факт выражается Statement
Instance, связывающим Values с Roles этого Statement. Statement само может
использоваться как Value (DEF-007), не теряя своей семантики отношения.

Human-readable specification: RFC-003.

## DEF-005 Role
Именованная позиция участия внутри Statement.

Role определяет только способ участия Value в конкретном Statement и не имеет
самостоятельной семантики вне этого Statement.

Human-readable specification: RFC-004.

## DEF-006 Statement Instance
Адресуемый экземпляр одного Statement, в котором каждой Role назначено ровно
одно Value и который явно участвует в Semantic Model.

Структурно допустимое назначение Values ролям Statement само по себе не
порождает Statement Instance. Statement Instance существует в Semantic Model
тогда и только тогда, когда оно соответствует своему Statement и используется
в модели как выраженный семантический факт либо как Value другого Statement
Instance.

Human-readable specification: RFC-005.

## DEF-007 Value
Семантический элемент, назначенный Role в Statement Instance.

Value не является отдельным видом объекта Semantic Core: Value может быть
Entity, Statement либо Statement Instance. Использование элемента как Value не
создаёт дополнительной семантики и не изменяет семантику, уже определённую его
видом; знания об элементе выражаются посредством Statement Instance.

Human-readable specifications: RFC-004, RFC-005.

## DEF-008 Constraint
Правило, ограничивающее допустимые модели.

Human-readable specification: RFC-006.

## DEF-009 Hierarchical Identifier Path (HIP)
Упорядоченный иерархический путь, однозначно адресующий один семантический
элемент в пределах Semantic Model.

Полный HIP является нормативным идентификатором адресуемого элемента.
Внутренние ключи, указатели и иные идентификаторы реализации не являются HIP
и не входят в Semantic Core.

Human-readable specification: RFC-016.

## DEF-010 Addressability
Свойство семантического элемента, позволяющее однозначно ссылаться на него в
пределах Semantic Model посредством его нормативного идентификатора.

Для Entity, Statement и Statement Instance нормативным идентификатором является
полный HIP (DEF-009). Addressability не определяет предметно-семантическую
идентичность элемента.

Human-readable specification: RFC-016.
