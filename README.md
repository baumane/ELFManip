# ELFManip

This was used as part of a larger project that needed the ability to add sections/segments to ELF executbles.
With that being said, it was built with a very specific usecase in mind and thus exposes limited functionality.

This is not indended to replace `objcopy`. Instead, it provides additional features.

Check the examples folder for a few simple examples.

# Limitations

- Known to work for *most* 32-bit ELF executalbes.
- Cannot add a segment without adding a corresponding section (one-to-one, see example).
- Requires section headers to be present and be ordered by address. This can be eliminated with some engineering.

# Installation

`python setup.py install`
