# Zen and the Art of Scientific Software Maintenance

One of the core principles of modern scientific software is to bring the best practices from
software engineering into the realm of scientific and research software. In this guide we
attempt to lay out those principles in the clearest way possible.

## Zen
- Make no unnecessary assumptions - use physics based formulae whenever possible over empirical
  relations.
- Clearly state all assumptions.
- Never depend on inputs with certain units.
- Function and class names should be spelled without abbreviation.
  (i.e. `equivalent_potential_temperature`, not `theta_e`)
- A single letter variable name is not acceptable for anything other than a counter. Variables
  should be spelled without abbrevation. (i.e. `temperature`, not `T` or `temp`)
- Vectorize calculations where possible - nested loops are the last resort.
- Generalize as much as possible, but no more.
- Users come first: API design, discoverability, and configurability are paramount.
- All contributions should cite the relevant literature - no constants or calculations that
  simply "appear".
- "That's how we've always done it" is not a citation.
- "That's how $LEGACY_SOFTWARE did it" is not a citation.
- Slide decks are not a citation.
- Compare against legacy calculations when possible.
- In five years will the [API](http://python.apichecklist.com) remain extensible?
- Be Pythonic - Python is awesome, write awesome code with it.
- Leave breadcrumbs for others. Explain why things are done and make useful git commit messages
  that do not require a decoder ring.
- Clean up your git history before merging.
- Is it good for the community?

## Projects Following the Zen
- [MetPy](https://github.com/Unidata/MetPy)

## Contributing
Is your project following the Zen? Add it to the list via a PR or file an
issue! We're trying to keep these guidelines short and sweet, but feel free
and propose additions.

## Contact
Have thoughts? You can contact me at jleeman@ucar.edu
