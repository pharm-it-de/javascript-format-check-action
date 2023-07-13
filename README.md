# JavaScript Code Format Check

This GitHub Action checks the code format of JavaScript files in your repository using Prettier and ESLint. It ensures that your code follows consistent formatting rules and adheres to best practices.

## Usage

```yaml
steps:
      - name: Use Code Format Check action
        uses: pharm-it-de/javascript-format-check-action@main
```

It is recommended to include this action in your workflow before any other actions that run tests or perform further processing on your JavaScript code. By checking the code format first, you can identify and fix formatting issues before running additional tasks.

## Inputs
### prettier-config-path
The prettier-config-path input allows you to specify the path to your Prettier configuration file. By default, it assumes that the configuration file is named .prettierrc.json and located in the root directory of your repository.
If your Prettier configuration file has a different name or is located in a different path, you can provide the custom path using the prettier-config-path input. For example:

```yaml
steps:
      - name: Use Code Format Check action
        uses: pharm-it-de/javascript-format-check-action@main
        with:
          prettier-config-path: 'path/to/.prettierrc.json'
```
