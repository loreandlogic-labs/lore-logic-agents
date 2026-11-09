# Ewan

## Goal for this program

Make the career shift into applied AI engineering, with a portfolio project to show for it.

## Flagship project (under consideration)

**Python coding helper, written from scratch**: a terminal app that works inside one project folder and helps find and fix bugs in Python code.

### Components

- **Agent loop**: written by hand, with no framework.
- **Tools**:
  - list files
  - read a file
  - run the tests
  - edit a file (only after asking first)
- **Modes**:
  - **Fix mode**: finds and repairs a bug.
  - **Tutor mode**: gives a hint without handing over the answer, the way Boot.dev does.

### Plan

- **First:** build the agent loop and the four tools, then the fix and tutor modes.
- **Later:** wrap the tools in my own MCP server so Claude Code can use them too.

### Evals

- An eval set of about 20 small buggy Python programs, written from my Boot.dev chapters (for example an off-by-one loop, a wrong dictionary key, a missing return), each with its own tests.
- **Fix mode:** do the tests pass after the fix?
- **Tutor mode:** does the hint leak the answer?
