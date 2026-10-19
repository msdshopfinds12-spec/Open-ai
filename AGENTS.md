# AGENTS.md

## Project purpose
This repository implements an AI-agent or automation workflow. Prioritize correctness, traceability, and safe iteration.

## Working conventions
- Keep changes small, focused, and easy to review.
- Favor explicit and readable logic over “clever” orchestration.
- Follow the repo’s existing structure and naming patterns.
- Avoid introducing new frameworks, tools, or dependencies without strong justification.
- Preserve backward compatibility unless the task explicitly requires breaking changes.

## Development workflow
- Understand the root cause before patching a bug or adding behavior.
- Prefer the narrowest validation command for the changed area.
- Keep changes scoped to the task at hand and avoid unrelated refactors.
- Document any new configuration, prompts, environment variables, or dependencies.
- Log or trace operational behavior when debugging agent workflows.

## AI-agent / automation guidance
- Treat prompts, tool calls, and orchestration logic as code.
- Keep agent behavior deterministic and explainable where possible.
- Avoid hidden side effects in tool execution or task chaining.
- Validate assumptions against repo logic and existing patterns before changing orchestration.
- Preserve user intent and constraints in prompt or workflow logic.

## Testing
- Add or update tests for bug fixes and new agent behaviors.
- Prefer focused validation around changed workflows or tool interactions.
- Fix root causes instead of masking failures in downstream logic.

## AI usage guidance
- Do not invent tools, APIs, prompt formats, or config values.
- Verify external behavior from repo code or documentation before assuming it.
- Keep patches minimal and aligned with the repository’s architecture.
- Be careful with retries, concurrency, and failure handling in automated flows.

## Quality bar
- Code should be readable, maintainable, and intentionally scoped.
- Relevant validation should pass before completion.
- Error handling, prompts, and agent flow logic should be explicit and reviewable.
