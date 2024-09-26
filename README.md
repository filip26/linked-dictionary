# Linked Dictionary

Yet another, but a very simple concept to turn tree data structures into Linked Data based on plain key-value dictionaries. That's it.

### Goals
 * simplicity
 * dictionaries generation
 * unambiguity
 * processing speed
 * language, serialization format, agnostic


## Linked Dictionary and JSON-LD

Linked dictionary is not a JSON-LD alternative. JSON-LD provides a full feature set to transform general JSON into/from RDF. Linked dictionary intentionally provides only basics, a simple mapping, and can serve only to a limited subset of JSON-LD use-cases.

| Feature | Linked Dictionary | JSON-LD |
| --- | --- | --- |
| Model  | Tree | Graph |
| Inline Definitions | ❌ | ✅ |
| Composability | ❌ |  ✅  (`@context` array, `@included`) | 
| Transformations | ❌ |  ✅  |
| Term Redefinition Resilience |  ✅  |  ✅ (`@protected`) |
| Term Definition Reflection | ✅ | ❌ (standard JSON-LD algorithms do not provide information about source of a term definition) |
| Term Definition Source Unambiguity  | ✅ | ❌ |
| Agnostic |  ✅ (a concept on how to annotate a tree structure with the use of dictionary structures) |  ❌ |
| Complexity | Low | Medium to High |




