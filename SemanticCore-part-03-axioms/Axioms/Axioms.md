# Axioms

## AX-001 Addressability
Каждая Entity и каждый Statement Instance являются индивидуально адресуемыми.

## AX-002 Role Value
Каждое вхождение Role имеет ровно одно значение.

## AX-003 Value Domain
Значением Role может быть либо Entity, либо Statement Instance.

## AX-004 Statement Structure
Statement определяет множество допустимых Role.

## AX-005 Instance Conformance
Каждый Statement Instance соответствует ровно одному Statement.

## AX-006 Theory Neutrality
Semantic Core не определяет идентичность, эквивалентность и уникальность объектов. Эти свойства задаются Theory.

## AX-007 Value Semantic Neutrality
Semantic Core не определяет внутреннюю семантику Value. Знания о Value
выражаются посредством Statement Instance.

## AX-008 Explicit Instance Existence
Структурно допустимое назначение Values ролям Statement не создаёт Statement
Instance автоматически. Statement Instance существует в Semantic Model тогда
и только тогда, когда оно соответствует своему Statement и явно участвует в
модели как выраженный семантический факт либо как Value другого Statement
Instance.

## AX-009 Presumption of Non-Identity
Два отдельно адресуемых семантических элемента считаются различными, пока
Theory явно не установит их семантическую идентичность посредством Statement
Instance. Совпадение структуры, значений, представления или иных наблюдаемых
свойств само по себе не устанавливает идентичность.
