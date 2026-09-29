# open-code-lab

Personal lab to get up and running with OpenCode, as well as how to build an harness around it

## Setup

Prefer installing globally with `pnpm`. The bash install script seems to leave many dangling dependencies.

```bash
pnpm install -g @opencode/cli --allow-build 
```

## Initial usage

Open a terminal window to run the cli:

```bash
opencode
```

Additionally, pass the workspace/working directory to change the working space.

```bash
opencode ~/Workspaces/Projects/cats
```

## Model selection

Type /models to list available models to use. Enter to select one.
