# spec-kit-presets

Spec Kit presets by fdcastel.

This repository contains [Spec Kit](https://github.com/github/spec-kit) presets that extend or customize the Spec-Driven Development workflow.

A preset is a package of custom templates and agent commands that transforms how spec-kit agent commands behave — replacing the default output style, terminology, and structure without changing any tooling.

## Available Presets

| Preset | Description |
|--------|-------------|
| [vscode-ask-questions](vscode-ask-questions/) | Enhances the clarify command to use `vscode/askQuestions` for batched interactive questioning, reducing API request costs in GitHub Copilot |

## Usage

Add this catalog URL to your Spec Kit configuration:

```
https://raw.githubusercontent.com/fdcastel/spec-kit-presets/main/catalog.json
```

Then install a preset with the Spec Kit CLI:

```bash
specify preset add --from https://github.com/fdcastel/spec-kit-presets/releases/download/<preset>-v<version>/<preset>.zip
```

Or from a local clone:

```bash
specify preset add --dev ./<preset>
```

You can also browse individual presets by navigating to their directory and reading the README for more details.

## Cheatsheet

To install the latest `vscode-ask-questions`
```powershell
specify preset add --from "https://github.com/fdcastel/spec-kit-presets/releases/download/vscode-ask-questions-v1.0.0/vscode-ask-questions.zip"
```

## More Information

See the [Spec Kit README](https://github.com/github/spec-kit/blob/main/README.md) for more information about Spec Kit and its preset system.

## License

MIT
