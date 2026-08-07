# Derived Properties

## DP-001 Statements about Semantic Elements
Из AX-003 следует, что Entity, Statement, Role и Statement Instance могут быть
значениями Role. Следовательно, единый механизм Statement / Statement Instance
допускает семантические утверждения о каждом базовом семантическом элементе.

---

## DP-002 Recursive Modeling
Так как Statement Instance является допустимым значением Role,
уровень вложенности модели принципиально не ограничен Semantic Core.

---

## DP-003 Presentation Equivalence
Из INV-001 и INV-002 следует, что любые канонические представления
описывают одну и ту же семантическую модель.

---

## DP-004 Theory Extensibility
Из DEC-005 и INV-006 следует, что новые теории могут вводить собственные
правила без изменения Semantic Core.

---

## DP-005 Primitive Sufficiency
Если конструкция выражается существующими примитивами,
введение нового примитива не требуется.

---

## DP-006 Implementation Freedom
Из разделения семантики и представления следует,
что формат хранения, API и способ сериализации
не являются частью стандарта Semantic Core.
