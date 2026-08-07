# Axioms

## AX-001 Addressability
Каждая Entity, каждый Statement и каждый Statement Instance являются
индивидуально адресуемыми.

## AX-002 Role Value
Каждое вхождение Role имеет ровно одно значение.

## AX-003 Value Domain
Значением Role может быть Entity, Statement либо Statement Instance.

## AX-004 Statement Structure
Statement определяет множество допустимых Role.

## AX-005 Instance Conformance
Каждый Statement Instance соответствует ровно одному Statement.

## AX-006 Theory Neutrality
Semantic Core не определяет предметно-семантическую идентичность, эквивалентность
или уникальность отдельных элементов модели. Эти отношения задаются Theory.

Core может определять собственные референциальные и адресные инварианты, а
также критерии сохранения и эквивалентности Semantic Model как целого,
необходимые для однозначной адресации, преобразований и conformance. Такие
правила не устанавливают предметную идентичность отдельных элементов.

## AX-007 Value Semantic Neutrality
Использование семантического элемента как Value не создаёт для него
дополнительной семантики и не изменяет семантику, уже определённую его видом.
Знания об элементе как предмете утверждений выражаются посредством Statement
Instance.

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
## AX-010 Hierarchical Addressing
Каждая Entity, каждый Statement и каждый Statement Instance адресуются полным
Hierarchical Identifier Path (HIP), уникальным в пределах Semantic Model. HIP
определяет
нормативный путь к элементу, но не способ его внутреннего хранения или поиска.
## AX-011 Statement-Centered Semantics
В базовом механизме Semantic Core семантика отношения задаётся только Statement.
Role задаёт позицию участия внутри своего Statement и не вводит самостоятельной
семантики. Statement Instance не определяет новое отношение, а выражает
конкретный семантический факт, связывая Values с Roles ровно одного Statement.

