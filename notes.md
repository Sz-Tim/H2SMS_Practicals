# Rendering

The project is set up with two profiles: `man` and `key`. 

The file `_quarto.yml` controls global options, with the profile-specific options specified in `_quarto-man.yml` and `_quarto-key.yml`.

To render the key, open the terminal and run:

> quarto render --profile="key"

To render the version for the students, run:

> quarto render --profile="man"

# Publishing

I think it's easiest to publish by setting the `QUARTO_PROFILE`.

To publish the key, run:

> export QUARTO_PROFILE=key
> quarto publish quarto-pub

To publish the version for students, run:

> export QUARTO_PROFILE=man
> quarto publish quarto-pub



