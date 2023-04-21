# Miscellaneous Notes

## Vision (?)

The core idea of the _demonator_ toolset is to enter a multi-screen,
multi-device, multi-media environment that allows the author to focus on the
core textual source representation of the system, while the various renderings
and assets are live compiled, updated, and displayed for visual confirmation of
the state of the system described.

The textual source representation allows expression and refinement of both
narrative and technical / structural descriptions of the system, and of
representative interactions with the system. These "representative interactions"
are the reason the toolset is called _demonator_, since they are built-in
demonstrations of the system's function.

You'll find a lot of inspiration for these interactions in tools like Cucumber,
etc., which encourage describing a system in "executable specifications".
Cucumber (as far as I remember), describes how the system should behave, and
uses these descriptions to generate documentation and scaffolding for tests
which verify this behaviour

I intend for the _demonator_ tools to also describe essential aspects of the
system's construction, and provide scaffolding for implementation, and other
kinds of documentation not offered by Cucumber, et al.

For example, while describing a particular interaction, an author might mention
a number of domain objects. From those mentions, the tools should generate code
and API stubs for the domain objects, scaffolding for UI components for the
objects, placeholder entries in the domain dictionary for the author to describe
the objects more thoroughly, etc.

Over time, as the author refines the domain objects, the tools should keep the
generated artifacts up to date - adding a representative icon to an object
should push that icon to everywhere an icon is useful (the dictionary, Figma
diagrams of workflows, etc.)

The author should thus be able to continuously "zoom in and out" of the system
description, sketching out narrative descriptions and placeholders, establishing
domain objects and interactions by mention, etc., until there are enough pieces
in place to describe enough of the system to begin implementing and testing
aspects of it.

## TODO

* discuss sliding levels of detail, declarative vs. imperative, etc. (esp. in
  context of [Writing better
  Gherkin](https://cucumber.io/docs/bdd/better-gherkin/)).
