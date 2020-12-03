# ge_talk_2020

Check the `presentation.ipynb` notebook for the presentation. Or the corresponding `html` slides.

## Build the talk yourself

Install the virtual environment with [poetry](https://python-poetry.org/): Get poetry and then in this
folder run:

```shell script
poetry install
``` 

Then the simplest way to build and serve the slides is:
```shell script
jupyter nbconvert presentation.ipynb --to slides --post serve 
```

For some theme/font control build the slide with something like this:
```bash
jupyter nbconvert presentation.ipynb --to slides --post serve 
--SlidesExporter.reveal_theme=serif 
--SlidesExporter.reveal_scroll=True 
--SlidesExporter.reveal_transition=none
```
___
NB: if you do not have the virtual environment activated, add `poetry run` before the commands!
