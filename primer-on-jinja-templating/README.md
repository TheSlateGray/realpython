# Primer on Jinja Templating

This repository holds the code from the Real Python [Primer on Jinja Templating](https://realpython.com/primer-on-jinja-templating/) tutorial.

## Dependencies

You should first create a virtual environment:

```console
$ python -m venv venv
$ source venv/bin/activate
```

You can then install Jinja and Flask with `pip`:

```console
(venv) $ python -m pip install Jinja2 flask
```

Alternatively, you can install the pinned dependencies from `requirements.txt`:

```console
(venv) $ python -m pip install -r requirements.txt
```

This command will install the versions used in the tutorial of Jinja, Flask, and the code formatting tools.

## Run the Web App

You can start your Flask development server by running `app.py` as a script:

```console
(venv) $ python app.py
```

To see your home page, visit `http://127.0.0.1:5000`.

## Things I learned
- Variables are set as `{{% variable_name %}}`.
- Conditionals are set as `{% if %}`, `{% else %}`, `{% endif %}` blocks.
- Loops are set in `{% for loop in loops %}` to `{% endfor %}` blocks.
- "Using `context` as a name for the collection that stores the variables for a template is a convention.
- `**` unpacks a dictionary. [PEP 448](https://peps.python.org/pep-0448/)
- "Variables can be modified by filters. Filters are separated from the variable by a pipe symbol `|` and may have optional arguments in parentheses. Multiple filters can be chained. The output of one filter is applied to the next." [Jinja Filters](https://jinja.palletsprojects.com/en/3.1.x/templates/#filters)
- "Note: In contrast to using Booleans in Python, you should write Booleans in Jinja in lowercase." 
- Use `{# comment #}` to comment out code in a Jinja HTML document, not `<!-- comment -->`.

## Original Author

- **Philipp Acsany**, I removed his email to not contribute to the scrapers.

## License

Distributed under the MIT license. See [`LICENSE`](../LICENSE) for more information.
