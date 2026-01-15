# Rendering

The project is set up with two profiles: `pub` and `key`. 

The file `_quarto.yml` controls global options, with the profile-specific options specified in `_quarto-pub.yml` and `_quarto-key.yml`.

To render the key, open the terminal and run:

> quarto render --profile="key"

To render the version for the students, run:

> quarto render --profile="pub"

# Publishing

I think it's easiest to publish by setting the `QUARTO_PROFILE`.

To publish the key, run:

> export QUARTO_PROFILE=key
> quarto publish quarto-pub

To publish the version for students, run:

> export QUARTO_PROFILE=pub
> quarto publish quarto-pub



