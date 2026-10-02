# open-code-lab

Personal lab to get up and running with OpenCode, as well as how to build an harness around it

## Setup

Prefer installing globally with `pnpm`. The bash install script seems to leave many dangling dependencies.

```bash
pnpm install -g @opencode/cli --allow-build=@opencode/cli
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

## Skills

Skills are loaded in the context window and extend the capabilities of agents. They follow a specific pattern and can either be declared in `.agents/skills` or `.opencode/skills` folders.

Each skill requires a folder that contains the **SKILL.md** file, following a specific pattern (see [hello-world skill](.agents/skills/hello-world/SKILL.md)). Skills can also contain scripts for extended control, such as other text or image sources.

A skill is either implictly run by the agent during the thinking/execution process, or explicitly using the `/skills` command.

## Commands

Commands are specific to opencode and need to be declared in `.opencode/commands` folder, using the command name as the file name (see [weather skill](.opencode/commands/weather.md)).

In essence, commands are short skills that are explicitly invoked.