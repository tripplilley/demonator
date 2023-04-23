# Example : Simple QR Code Inventory System

For a motivating example, we're going to describe a system which allows a person
to manage an inventory of personal property using the [@veatech.one
platform](https://veatech.one/platform/)

!> **NOTE:** Although it's tempting to use _demonator_ to build _demonator_,
we're not going to do that, because it's far too easy to make an infinite
funhouse mirror rabbit-hole ourobouros that way. Instead, we're going to capture
thoughts and ideas in these notes and use the example, itself, to explore and
exercise the tools.

This system has a few pieces we know of already:

- A mobile app we're going to build (React Native).
- A user signup / login mechanism:
    - Basic identity / auth services are provided by the platform - we need to
      integrate them into the app.
- A QR code scanner (integrated into the app)
- QR codes on labels:
    - The platform provides the data to go in the codes, which we feed into our
      labeling software, outside of the mobile app.
- A way to capture text about an inventory item (in the app).
- A way to capture photos of an inventory item (in the app).
- A way to indicate the designated location of an inventory item (i.e., where it
  _should_ be).

The job of _demonator_ is to allow us to collect these requirements and round
them out as we come to them, as we get more info, as we refine our ideas, etc.
We're describing the system in higher and higher resolution, until we ultimately
have working artifacts in our hands.

As we describe the system, _demonator_ should help us by collecting nouns,
verbs, adjectives, etc., and building a live glossary (the _Domain Dictionary_,
a repository for the system's [Ubiquitous
Language](https://martinfowler.com/bliki/UbiquitousLanguage.html)).
