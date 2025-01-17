# WASI URLs

A [WebAssembly System Interface](https://github.com/WebAssembly/WASI)
API for URLs.

### Current Phase

Phase 1

### Champions

- George Kulakowski
- Radu Matei

### Phase 4 Advancement Criteria

TODO before entering Phase 2.

## Table of Contents [if the explainer is longer than one printed page]

- [Introduction](#introduction)
- [Goals [or Motivating Use Cases, or Scenarios]](#goals-or-motivating-use-cases-or-scenarios)
- [Non-goals](#non-goals)
- [API walk-through](#api-walk-through)
  - [Use case 1](#use-case-1)
  - [Use case 2](#use-case-2)
- [Detailed design discussion](#detailed-design-discussion)
  - [[Tricky design choice 1]](#tricky-design-choice-1)
  - [[Tricky design choice 2]](#tricky-design-choice-2)
- [Considered alternatives](#considered-alternatives)
  - [[Alternative 1]](#alternative-1)
  - [[Alternative 2]](#alternative-2)
- [Stakeholder Interest & Feedback](#stakeholder-interest--feedback)
- [References & acknowledgements](#references--acknowledgements)

### Introduction

URLs are a very common, standardized vocabulary and interchage
type. This proposal defines a URL resource and operations on it.

### Goals [or Motivating Use Cases, or Scenarios]

#### Standard compliance

This proposal will adhere to the [WHATWG URL spec][whatwg-url-spec].

Concretely, this will mean using terminology as defined in that document.

Besides the WHATWG specification, there are a series of IETF RFCs
defining the syntax and semantics of URLs, as well as RFCs defining
constraints for specific schemes. Furthermore, various browser, OS,
and language standard library APIs define URL data types.

The choice to use the WHATWG specification is deliberate. TODO WHY

### Non-goals

This proposal will not include constructors or accessors tailored to
specific URL schemes defined by other RFCs, at least initially.

This proposal makes a URL a resource type. The overhead of the
resource abstraction is a cost that some use cases of URLs may not
want to pay.

### API walk-through

The WASI URL interface will contain a URL resource type and methods
for creating and consuming URL resources.

[Walk through of how someone would use this API.]

#### [Use case 1]

[Provide example code snippets and diagrams explaining how the API would be used to solve the given problem]

#### [Use case 2]

[etc.]

### Detailed design discussion

[This section should mostly refer to the .wit.md file that specifies the API. This section is for any discussion of the choices made in the API which don't make sense to document in the spec file itself.]

#### [Tricky design choice #1]

[Talk through the tradeoffs in coming to the specific design point you want to make.]

```
// Illustrated with example code.
```

[This may be an open question, in which case you should link to any active discussion threads.]

#### [Tricky design choice 2]

[etc.]

### Considered alternatives

[This section is not required if you already covered considered alternatives in the design discussion above.]

#### [Alternative 1]

[Describe an alternative which was considered, and why you decided against it.]

#### [Alternative 2]

[etc.]

### Stakeholder Interest & Feedback

TODO before entering Phase 3.

[This should include a list of implementers who have expressed interest in implementing the proposal]

### References & acknowledgements

#### Specifications

The [WHATWG URL spec][whatwg-url-spec] defines URLs, and an API that
substantially informs this one.

#### Thanks

Many thanks for valuable feedback and advice from:

- [Person 1]
- [Person 2]
- [etc.]

[whatwg-url-spec]: https://url.spec.whatwg.org/
