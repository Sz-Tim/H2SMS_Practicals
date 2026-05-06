# Project profiles

The project is set up with two profiles: `man` and `key`. 

The file `_quarto.yml` controls global options, with the profile-specific options specified in `_quarto-man.yml` and `_quarto-key.yml`.

The manual and key can be re-rendered and published by running

> bash publish_man.sh

and

> bash publish_key.sh

The contents of the key (`_quarto-key.yml`) should be updated session by session throughout the semester as solutions are made available.



# Rendering separately

To render the version for the students, run:

> quarto render --profile="man"

To render the key, open the terminal and run:

> quarto render --profile="key"



# Publishing separately

I think it's easiest to publish by setting the `QUARTO_PROFILE`.

To publish the version for students, run:

> export QUARTO_PROFILE=man
> quarto publish quarto-pub

To publish the key, run:

> export QUARTO_PROFILE=key
> quarto publish quarto-pub


