# Scope and Boundaries

## In scope
AI-SECF governs how project-specific Claude Code configuration is:
- discovered and planned;
- structured and scoped;
- written and referenced;
- generated and revised;
- validated and tested;
- secured and approved;
- versioned, reviewed, and retired.

## Out of scope
AI-SECF is not a general software engineering governance framework. It does not itself mandate:
- application architecture or technology choices;
- coding style or implementation patterns;
- product requirements or delivery methodology;
- business risk management, regulatory compliance, or operational SLAs;
- test strategy for the product, except configuration validation and instructions about how Claude should invoke existing project tests.

A target project may already have standards for these topics. AI-SECF may discover and accurately summarize them into Claude-facing instructions, but must not invent or replace them.

## Separation of concerns
1. **Project facts:** What the repository demonstrably contains.
2. **Project decisions:** Choices made by authorized project stakeholders.
3. **Claude instructions:** How Claude should use project facts and follow approved decisions.
4. **Claude runtime configuration:** Supported settings and extension mechanisms that affect Claude Code behavior.
5. **AI-SECF rules:** Universal requirements for creating and maintaining the above.

## Non-goals
- Maximize the number of files.
- Put the whole repository's documentation into CLAUDE.md.
- grant broad tool permissions for convenience.
- Create agents, skills, hooks, commands, or MCP servers merely because the feature exists.
- Treat generated configuration as correct without validation and human review.
