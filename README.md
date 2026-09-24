# nexodu.github.io

## What the repository is
This is an analysis of how the body mass(g) differs among the penguin species, including the mean, the median, and 
the standard deviation.

## What to install
- Quarto 1.10.18
- uv 0.12.17
- python 3.13.13
- R 4.6.1
- Git

## The exact commands, in order
git clone git@github.com:NexoDu/nexodu.github.io.git
cd nexodu.github.io
uv sync --locked
Rscript -e 'renv::restore(prompt = FALSE)'
uv run quarto render


## Where the build site lands
The website is saved in docs/posts/
Start the local server:
uv run python -m http:.server 8000 --directory docs


## Source of the Analysis
Data: [Palmer Penguins](https://allisonhorst.github.io/palmerpenguins/),
Data license: CC0
Palmer Station Antarctica LTER.
Package reference: Horst, A. M., Hill, A. P., and Gorman, K. B. (2020). palmerpenguins: Palmer Archipelago (Antarctica) penguin data. https://doi.org/10.5281/zenodo.3960218.