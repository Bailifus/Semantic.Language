# RFC-005: Statement Instance

Status: Draft

## Purpose

Определить семантику Statement Instance как экземпляра Statement.

## Scope

Документ описывает только Statement Instance.

## Definition

Statement Instance является конкретным экземпляром Statement, в котором каждой Role назначено значение.

## Normative Requirements

SI-001 Каждый Statement Instance ссылается ровно на один Statement.

SI-002 Каждый Role, определённый Statement, должен иметь значение в Statement Instance.

SI-003 Statement Instance не может содержать Role, отсутствующие в Statement.

SI-004 Значением Role может быть только Entity или Statement Instance.

SI-005 Statement Instance является адресуемым объектом Semantic Model.

## Non-goals

- порядок хранения;
- временные аспекты;
- контроль целостности Theory.

## Rationale

Statement Instance представляет конкретный семантический факт, соответствующий структуре Statement.

## References

DEF-006
AX-002
AX-003
AX-005
