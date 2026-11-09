# Lochlan

## Goal for this program

TODO: add my goal for the program.

## Flagship project (under consideration)

**Agent red-team harness**: a reusable tool that attacks AI agents to find security weaknesses before real attackers do.

### Components

- **Attacker agent**: generates attacks such as:
  - hidden instructions in user input, or in files and web pages the agent reads (prompt injection)
  - tricking the agent into misusing a tool
  - getting the agent to leak its instructions or secrets
- **Target adapter**: connects to the agent under test through its own MCP server.
- **Judge agent**: decides whether each attack worked.
- **Report agent**: writes up the findings and recommended fixes.

### Plan

- **Weeks 5–6:** build my own small target agent and attack it first.
- **After that:** point the harness at teammates' flagship projects.

### Evals

- Attack success rate for each attack category.
- Judge agreement: check how often the judge's verdicts match my own hand-labelled verdicts.
