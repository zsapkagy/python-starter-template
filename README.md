# Install UV

[Install UV](https://docs.astral.sh/uv/configuration/installer/)

## Generate shell completion

[Generate shell completion](https://docs.astral.sh/uv/reference/cli/#uv-generate-shell-completion)

The following command could be added to the .bashrc file to generate shell completion for uv.

```
eval "$(uv generate-shell-completion bash)"
```

## Init UV

To initialize the project, run the following command

```
uv init
```

It will create a virtual environment and install the dependencies.

# Virtual Environments

If the virtual environment doesn't get selected, you can select it with the following steps:

1. Open Command Palette: Use the shortcut to open the Command Palette in VS Code.
2. Select Environment Command: Type and select `Python: Select Interpreter` to choose an existing interpreter or create a new virtual environment. See additional instructions how to work with Python interpreters in VSCode [here](https://github.com/microsoft/vscode-python/wiki/Setting-descriptions#pythondefaultinterpreterpath).

But the following VSCode settings should alreadyset the interpreter to the one in the `.venv` folder.

```
  "python.terminal.activateEnvironment": true,
  "python.defaultInterpreterPath": "${workspaceFolder}/.venv/bin/python",
```

# Repository structure

Check for more tips the following resources

- https://datalumina.clickup.com/docs/9015213037/d/h/8cnjezd-17675/ddd52c673443975
- https://github.com/datalumina/datalumina-project-template/blob/main/README.md
- https://github.com/daveebbelaar/langchain-experiments
- https://github.com/ArjanCodes/examples/tree/main/2024/vscode_python

## VsCode extensions and settings

```
.vscode/extensions.json
.vscode/settings.json
```

## Linting and formatting

We use [Ruff](https://github.com/astral-sh/ruff) for linting and formatting.

Check the `ruff.toml` file for [configuration](https://docs.astral.sh/ruff/configuration/).

```
ruff.toml
```

## Cursor rules

If you use Cursor, you can use the `.cursorrules` file to set your rules.

[Cursor directory](https://cursor.directory/)
