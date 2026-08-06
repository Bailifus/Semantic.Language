# RFC-000: Semantic Core Constitution

- **Status:** Draft — frozen bootstrap snapshot
- **Category:** Constitutional
- **Scope:** Entire Semantic Core standard
- **Version:** Part 01 / 2026-07-25

## 1. Purpose

Semantic Core is a technology-independent semantic modeling standard.

Its purpose is to define a minimal and compositional foundation for representing meaning in a form that can be implemented independently, serialized canonically, visualized, validated, and extended by theories without importing assumptions from a particular programming language, storage model, ontology formalism, user interface, or execution environment.

## 2. Authority of this document

This Constitution governs all normative documents of the Semantic Core standard.

A later RFC, definition, axiom, syntax rule, conformance rule, example, implementation note, or presentation convention must not contradict this document.

A proposal that requires violating a constitutional principle must amend this document explicitly rather than bypass it indirectly.

## 3. Separation of concerns

The standard separates four layers:

1. **Semantic Model** — defines meaning.
2. **Canonical Text** — the primary normative serialization of that meaning.
3. **Canonical Diagram** — a derived graphical representation of Canonical Text.
4. **Presentation** — non-canonical ways to display, navigate, group, hide, expand, collapse, color, or arrange semantic information.

Meaning exists only in the Semantic Model.

Canonical Text serializes the Semantic Model and is the normative source for its serialized form. Canonical Diagram represents Canonical Text graphically and must not introduce, remove, or override meaning.

Presentation may alter visibility and arrangement, but it must not alter or destroy the underlying semantics.

## 4. Minimality

Semantic Core follows the principle of parsimony.

A new semantic primitive may be introduced only after demonstrating that the required capability:

1. cannot already be expressed by composition of existing primitives;
2. is not merely a presentation concern; and
3. does not properly belong to a Theory.

Convenience alone is not sufficient justification for a new primitive.

Every primitive must be indispensable.

## 5. Conceptual purity

Every concept must be justified within the Semantic Core model itself.

Concepts must not be imported merely because they are familiar from another paradigm, notation, or implementation technology.

In particular, no proposal gains legitimacy merely by analogy with:

- object-oriented classes or inheritance;
- relational tables;
- RDF subject-predicate-object triples;
- UML constructs;
- programming-language types;
- database identifiers;
- graphical notation conventions.

External concepts may inspire analysis, but they do not become part of the standard without an independent semantic justification.

## 6. Theory extension

Semantic Core defines the minimal machinery required to express semantic structures.

Domain-specific meaning, identity rules, equivalence, uniqueness, conflict detection, inference, classification, validation policies, and other higher-order commitments belong to Theories unless explicitly proven to require Core support.

The Core must remain neutral where multiple coherent theories are possible.

## 7. Presentation independence

No semantic fact may depend on a particular visual layout, color, icon, indentation, screen size, interaction pattern, zoom level, or rendering technology.

Presentation may:

- hide information;
- reveal information;
- group or ungroup elements;
- collapse or expand structures;
- recolor elements;
- change layout;
- provide alternative navigation.

Presentation must never destroy, replace, or silently reinterpret semantic information.

## 8. Level of Detail

The normative term is **Level of Detail (LOD)**.

A presentation may expose different levels of detail. Increasing detail reveals semantics that already exist. It must not create new semantics or change existing semantics.

A user-interface implementation may call this behavior **Semantic Zoom**, but that term is non-normative.

## 9. Compositionality

Complex semantic structures should be expressible by composition of simpler structures.

Special cases should not receive dedicated primitives when ordinary composition is sufficient.

The meaning of a composite structure must be determined by its semantic constituents and the rules governing their composition, not by hidden implementation behavior.

## 10. Addressability and implementation neutrality

The Core may require semantic objects to be individually addressable.

Such addressability must not be confused with storage identity, memory address, database key, URI scheme, object reference, or any other implementation-specific identifier.

Storage, indexing, caching, lookup, persistence, and transport mechanisms are outside the Semantic Core unless separately standardized.

## 11. Semantic preservation

Any transformation claiming to preserve a Semantic Core model must preserve all semantic information defined by that model.

Lossless changes of notation, layout, ordering, encoding, grouping, or visibility are permitted when the original semantics remain recoverable in Canonical Text.

A Canonical Diagram is semantically preserving only when its source Canonical Text can be recovered without semantic loss.

A lossy transformation must identify itself as lossy and must not claim semantic equivalence.

## 12. Canonical representation hierarchy

Canonical Text is the primary normative serialization of a Semantic Model.

Canonical Diagram is a derived representation of Canonical Text, not an independent source of normative meaning. A diagram is canonically equivalent to its source only when conversion from Canonical Text to Canonical Diagram and back preserves the Canonical Text without semantic loss.

If Canonical Text and Canonical Diagram conflict or differ in interpretation, Canonical Text prevails.

Independent conforming implementations must be able to determine whether canonical representations denote the same semantic structure according to rules defined by later normative specifications.

Presentation artifacts are not part of canonical equivalence.

## 13. Engineering relevance

A proposed feature must solve a real semantic modeling problem.

The standard applies three filters in order:

1. **Occam's Razor** — is the proposal necessary?
2. **Lumberjack Test** — what concrete modeling work does it enable?
3. **API Test** — is the concept minimal, orthogonal, composable, and stable enough to expose as part of the semantic foundation?

A proposal that fails any filter should not enter the Core.

## 14. API principle

Semantic Core is treated as a minimal semantic API.

Therefore:

- primitives should be few;
- concepts should be orthogonal;
- composition is preferred over special cases;
- syntactic sugar does not belong to the Core;
- convenience belongs primarily to Presentation;
- expressiveness belongs primarily to Theory.

## 15. Evolution

The standard should evolve by explicit, reviewable decisions.

Normative changes must identify:

- the problem being solved;
- the affected principles and documents;
- rejected alternatives;
- non-goals;
- compatibility consequences;
- conformance consequences.

Existing normative meaning must not be changed accidentally through editorial rewriting.

## 16. Independence of axioms

Axioms must be minimized.

Every proposed axiom must be either:

- independent and necessary; or
- derivable from existing axioms and definitions.

A derivable proposition is not an axiom and should be recorded as a derived property.

## 17. Standardization objective

The objective is not merely to describe an author's intent.

The objective is to enable independent implementers to converge on compatible behavior.

Normative text must therefore avoid hidden assumptions, undefined terminology, implementation folklore, and reliance on examples as substitutes for rules.

## 18. Review discipline

Normative proposals should be reviewed as if by a standards committee.

Review must actively search for:

- contradictions;
- ambiguity;
- incompleteness;
- redundant primitives;
- hidden implementation assumptions;
- places where independent implementations could diverge.

New features should not be proposed until the insufficiency or inconsistency of the current model has been demonstrated.

## 19. Preservation discipline

Unrecorded decisions are considered lost.

Significant work must be preserved in versioned, non-overwritten artifacts.

The project should prefer small, coherent, reviewable archives over large undocumented leaps.

## 20. Non-goals of this Constitution

This document does not define:

- the complete set of Semantic Core primitives;
- formal axioms;
- normative definitions of Theory, Domain, Entity, Statement, Role, Constraint, or Statement Instance;
- identity or equivalence rules;
- concrete textual grammar;
- diagram syntax;
- serialization formats;
- storage models;
- query languages;
- editing APIs;
- inference engines;
- user-interface behavior;
- conformance test cases.

Those belong to later documents governed by this Constitution.

## 21. Rejected constitutional alternatives

### 21.1 Technology-first specification

Rejected because tying the semantic foundation to a programming language, database, graph store, or serialization format would make implementation details normative and reduce portability.

### 21.2 Ontology-first specification

Rejected because committing the Core to one theory of identity, equivalence, classification, or inference would prevent alternative coherent theories from using the same semantic foundation.

### 21.3 Presentation-driven semantics

Rejected because layout, icons, colors, and interaction patterns are unstable and implementation-specific. They may expose meaning but must not define it.

### 21.4 Feature-rich Core

Rejected because convenience primitives increase conceptual coupling, create overlapping representations, and make independent implementations more likely to diverge.

### 21.5 Informal evolution

Rejected because undocumented decisions and silent reinterpretations make a standard impossible to implement reliably.
