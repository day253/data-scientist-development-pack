# Data Scientist Development Pack

This extension pack packages some of the most popular (and some of my favorite) Python/Jupyter extensions.

## Extensions Included

* [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) - Linting, Debugging (multi-threaded, remote), Intellisense, code formatting, refactoring, unit tests, snippets, Data Science (with Jupyter), PySpark and more.
* [Black Formatter](https://marketplace.visualstudio.com/items?itemName=ms-python.black-formatter) - Code formatting using Black.
* [isort](https://marketplace.visualstudio.com/items?itemName=ms-python.isort) - Import sorting using isort.
* [Data Wrangler](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.datawrangler) - Data cleaning and preparation tool.
* [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) - Jupyter notebook support.
* [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) - Remote development.
* [YAML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-yaml) - YAML language support.
* [Even Better TOML](https://marketplace.visualstudio.com/items?itemName=tamasfe.even-better-toml) - TOML language support.
* [Sort Lines](https://marketplace.visualstudio.com/items?itemName=tyriar.sort-lines) - Sort lines of text.

## Usage

- **Python Language Server**: [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) is used as the Python language server. Note: If you've previously set a language server and want to try Pylance, make sure you've set "python.languageServer": "Default" or "Pylance" in your settings.json file using the text editor, or using the Settings Editor UI.

- **Integrated Import Sorting**: Once [isort](https://marketplace.visualstudio.com/items?itemName=ms-python.isort) extension is installed in Visual Studio Code, isort is automatically registered as an import organizer. You can use `Shift + Alt + O` to trigger the organize imports editor action. You can also trigger this from the quick fix available when imports are not organized.

- **Customizable isort Arguments**: You can customize the arguments passed to [isort](https://marketplace.visualstudio.com/items?itemName=ms-python.isort) by modifying the `isort.args` setting.

- **Import Sorting on Save**: You can enable import sorting on save for Python files by changing the `editor.codeActionsOnSave` setting. It also works alongside the [VS Code Black formatter extension](https://marketplace.visualstudio.com/items?itemName=ms-python.black-formatter) if you set the following settings:

```json
    "python.languageServer": "Pylance",
    "[python]": {
        "editor.defaultFormatter": "ms-python.black-formatter",
        "editor.formatOnSave": true,
        "editor.codeActionsOnSave": {
            "source.organizeImports": "explicit"
        }
    },
    "isort.args": [
        "--profile",
        "black"
    ],
```

## Want to see your extension added?

Open a PR and I'd be happy to take a look.

**Enjoy!**
