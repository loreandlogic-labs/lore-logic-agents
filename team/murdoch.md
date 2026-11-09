# Murdoch

## Program goal

Move into an AI engineering career by building a portfolio of real, working
agent systems and the skills to design, test and ship them.

## Flagship idea: Game economy auditor

An agent system that audits a game economy for design mistakes.

- **The data.** I design the economy for a fantasy crafting game as four
  tables: items, recipes, monster drops and shop prices. I plant about 15
  mistakes in it, for example:
  - a buy-craft-sell loop that makes free money
  - an item no one can obtain
  - an overpowered tier-1 sword
  - drop odds that add up to more than 100%
- **The tools.** An MCP server exposes the four tables to the agents.
- **The agents.** Specialist agents each hunt one kind of mistake: a loop
  finder, a reachability checker and a balance checker. A report agent then
  writes up suggested fixes for a lead designer.
- **The evals.** The eval suite doubles as my UAT plan. Each planted mistake is
  a test case with an expected result, so I can measure which mistakes the
  system catches and which it misses.
