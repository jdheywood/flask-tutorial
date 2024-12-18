# Tutorial from Flask website

Followed the tutorial here: https://flask.palletsprojects.com/en/stable/tutorial/

Only difference is I used [uv](https://github.com/astral-sh/uv) to manage dependencies, which adjusts the various commands slightly (but not much) - it is super-fast though, worth the pain to migrate to I reckon.

```zsh
uv init v1

cd v1

uv add flask

uv flask --app flaskr run --debug

uv run flask --app flaskr init-db    

uv --help   

uv sync

uv add pytest coverage

uv run pytest 

uv run coverage run -m pytest

uv run coverage report

```
