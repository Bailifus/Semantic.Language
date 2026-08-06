# RFC-005: Statement Instance

Status: Draft

## Purpose

Определить семантику Statement Instance как экземпляра Statement.

## Scope

Документ описывает только Statement Instance.

## Definition

Canonical definitions: DEF-006 (Statement Instance), DEF-007 (Value).

Statement Instance является конкретным экземпляром Statement, в котором каждой Role назначено Value.

Value — объект, назначенный Role. Semantic Core не приписывает Value внутреннюю
семантику; знания о нём выражаются посредством Statement Instance.

## Normative Requirements

SI-001 Каждый Statement Instance ссылается ровно на один Statement.

SI-002 Каждый Role, определённый Statement, должен иметь значение в Statement Instance.

SI-003 Statement Instance не может содержать Role, отсутствующие в Statement.

SI-004 Значением Role может быть только Entity или Statement Instance.

SI-005 Statement Instance является адресуемым объектом Semantic Model.

SI-006 Semantic Core не должен приписывать Value внутреннюю семантику вне
Statement Instance, в которых оно участвует.

## Non-goals

- порядок хранения;
- временные аспекты;
- контроль целостности Theory.

## Rationale

Statement Instance представляет конкретный семантический факт, соответствующий структуре Statement.
Value участвует в таком факте, но не несёт встроенного описания собственного
смысла. Любые знания о Value должны быть выражены тем же механизмом — через
Statement Instance.

## References

DEF-006
AX-002
AX-003
AX-005
AX-007
DEC-008
