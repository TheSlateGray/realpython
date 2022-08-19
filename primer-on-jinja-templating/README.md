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

## Original Author

- **Philipp Acsany**, E-mail: [philipp@realpython.com](philipp@realpython.com)

## License

Distributed under the MIT license. See [`LICENSE`](../LICENSE) for more information.