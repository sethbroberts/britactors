# Hopkins-McKellan-Jacobi Classifier

My first attempt at a machine learning API, using a pre-calculated model trained using Google Image data. This model classifies images into the following categories: Anthony Hopkins, Ian McKellan, Derek Jacobi.

This is a copy of Simon Willison's repo [cougar-or-not](https://github.com/simonw/cougar-or-not). Simon does lots of brilliant [work](https://www.youtube.com/watch?v=pTr1uLQTJNE).

The model is `export.pkl` - an 87MB file.

The notebook `britactors.ipynb` shows how the model was trained, using [fastai](https://github.com/fastai/fastai).

`actor.py` is a very tiny [Starlette](https://www.starlette.io/) API server which simply accepts file image uploads and runs them against the pre-calculated model.

It also accepts a URL to an image, e.g. https://tvguide1.cbsistatic.com/mediabin/showcards/celebs/a-b/thumbs/anthony-hopkins-140365_828x1104.png

The `Dockerfile` means the entire thing can be deployed to [Zeit Now](https://zeit.co/now) or any other container hosting service.

## Examples
