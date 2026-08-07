# RFC-005: Statement Instance

Status: Draft

## Purpose

Определить семантику Statement Instance как экземпляра Statement.

## Scope

Документ описывает только Statement Instance.

## Definition

Canonical definitions: DEF-006 (Statement Instance), DEF-007 (Value).

Statement Instance является адресуемым экземпляром одного Statement, в котором
каждой Role назначено ровно одно Value и который явно участвует в Semantic
Model.

Корректное назначение Values ролям Statement описывает возможный экземпляр, но
не создаёт Statement Instance автоматически. Экземпляр существует в Semantic
Model только тогда, когда он используется как выраженный семантический факт
либо как Value другого Statement Instance.

Value — объект, назначенный Role. Semantic Core не приписывает Value внутреннюю
семантику; знания о нём выражаются посредством Statement Instance. Сам
Statement Instance не задаёт новое отношение: он выражает семантику своего
Statement для конкретного набора назначенных Values.

## Normative Requirements

SI-001 Каждый Statement Instance ссылается ровно на один Statement.

SI-002 Каждый Role, определённый Statement, должен иметь значение в Statement Instance.

SI-003 Statement Instance не может содержать Role, отсутствующие в Statement.

SI-004 Значением Role может быть только Entity или Statement Instance.

SI-005 Statement Instance является адресуемым объектом Semantic Model.

SI-006 Semantic Core не должен приписывать Value внутреннюю семантику вне
Statement Instance, в которых оно участвует.

SI-007 Statement Instance существует в Semantic Model тогда и только тогда,
когда оно удовлетворяет SI-001—SI-004 и явно участвует в модели как выраженный
семантический факт либо как Value другого Statement Instance.

SI-008 Statement Instance не определяет самостоятельную семантику отношения, а
выражает семантику своего Statement посредством назначения Values его Roles.

## Non-goals

- порядок хранения;
- механизм добавления и удаления Statement Instance;
- временные аспекты;
- контроль целостности Theory.

## Rationale

Statement Instance представляет конкретный семантический факт, соответствующий
структуре Statement. Возможность корректно назначить Values всем Roles ещё не
означает, что такой экземпляр существует в модели. Явное участие отделяет
реальные элементы Semantic Model от неограниченного множества структурно
возможных, но нигде не используемых экземпляров.

Value участвует в таком факте, но не несёт встроенного описания собственного
смысла. Любые знания о Value должны быть выражены тем же механизмом — через
Statement Instance. Благодаря этому все семантические факты используют один и
тот же механизм: Statement задаёт отношение, а Statement Instance связывает
конкретные Values с его Roles.

## References

DEF-006
DEF-010
AX-002
AX-003
AX-005
AX-007
AX-008
DEC-008
DEC-009
AX-011
DEC-012
