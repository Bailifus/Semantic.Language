# Examples

## EX-001 Простое утверждение

Theory: Family

Statement: Parent

Roles:
- parent
- child

Instance:
Parent(parent=Alice, child=Bob)

---

## EX-002 Утверждение об утверждении

Statement:
Verified

Roles:
- statement
- reviewer

Instance:
Verified(
  statement = Parent(parent=Alice, child=Bob),
  reviewer = Carol
)

---

## EX-003 Две независимые теории

Theory A:
Employee(Person, Company)

Theory B:
Citizen(Person, Country)

Semantic Core не навязывает связи между теориями.

---

## EX-004 Один Entity в нескольких утверждениях

Entity:
Alice

Используется одновременно в:
- Parent
- Employee
- Citizen

Entity остается одним и тем же адресуемым объектом.
