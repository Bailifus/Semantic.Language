# Conformance

## CF-001 Core Primitives
Реализация должна поддерживать все примитивы Semantic Core.

## CF-002 Role Semantics
Реализация должна интерпретировать присвоение значения роли одинаково.

## CF-003 Canonical Representation Hierarchy
Canonical Text должен быть первичным нормативным представлением модели.
Canonical Diagram должен быть выводим из Canonical Text и допускать восстановление
его семантики без потерь.

## CF-004 Theory Separation
Теории не должны изменять семантику примитивов Core.

## CF-005 Presentation Independence
Представление не должно влиять на смысл модели.

## CF-006 Addressability
Каждая Entity и каждый Statement Instance должны иметь устойчивую адресацию
в рамках реализации.

## CF-007 Extension Safety
Расширения допустимы только без нарушения требований CF-001...CF-006.
