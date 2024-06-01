JSON schema for `.vscode/launch.json` files.

The main motivation behind this is to get code completion and documentation
(`hover`) when using the `vscode-json-languageserver` while editing debug
configurations in an editor that is not `vscode` and doesn't have debug adapter
specific vscode-extensions installed.


## Usage

Add a `$schema` line to your `.vscode/launch.json` file:

```json
{
   "$schema": "https://raw.githubusercontent.com/mfussenegger/dapconfig-schema/master/dapconfig-schema.json",
   "version": "0.2.0",
   "configurations": [
   ]
}
```

Ensure `vscode-json-language` is running and you should get property
completion, hover/documentation and validation.


## Contributions

PRs that extend the schema with properties for more debug adapters are welcome
