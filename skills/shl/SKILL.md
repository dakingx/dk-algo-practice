---
name: shl
description: |
  Solve SHL algorithm programming problems. Use this skill when the user mentions SHL problems. This skill handles the full workflow: parsing the problem statement, writing solution code, and running test cases until all pass.
metadata:
   author: Daking
   version: 0.2.0
---

# SHL Algorithm Problem Solver

## Workflow

Follow these steps in order. Do not skip steps.

### Step 1: Understand the Problem

1. **Understand the user's requirements and the problem.** Read the provided problem statement, relevant attachments, and `references/question_template.md`. Identify the intended task,input/output behavior, constraints, and examples where provided. At any point during understanding or conversion, ask the user to clarify uncertainties, missing details that affect the solution, or conflicting information before proceeding with the affected work. Do not invent requirements or silently make assumptions.

2. **Convert to the question template when needed.** Organizethe understood content using the structure in `references/question_template.md`, preserving the original meaning. All template sections and subsections are recommended, not mandatory; do not fabricate content just to fill them. Identifyany omitted sections or details for the user to confirm. If the provided content already follows the template structure, skip conversion, but not the final confirmation below.

3. **0btain explicit confirmation of the final question.** Present the complete final question to the user, whether converted or already formatted. Ask the user to confirm both the question content and any omitted template sections or details. If the user requests changes, clarify any new uncertainties revise the question, and present it again for confirmation. Do not proceed to Step 2 or write solution code until all uncertainties are resolved and the user explicitly confirms the final question, including any omissions.

### Step 2: Write the Solution

Write the solution following the template in `assets/code_template.md` (load it before writing).s

<python_version>3.7</python_version>

Key rules:

- **Python ${python_version}** only. No walrus operator, no dataclasses, no typing features beyond ${python_version}.
- **No third-party libraries.** Only use the Python standard library.
- **Naming**: Use `snake_case` for functions and variables. Choose descriptive, semantic names.
- **Comments**: Add brief English comments (1-2 sentences) at key steps to explain the algorithm logic.

Save the solution file to the path the user specifies, or default to `solution.py` in the current working directory.

### Step 3: Run and Verify

1. Run the solution against the example test cases from the problem:
   ```bash
   python3 solution.py < test_input.txt
   ```
   Create `test_input.txt` from the problem's example input.

2. Compare output against expected output.

3. If any test case fails:
   - Analyze the failure (wrong answer, timeout, runtime error, etc.)
   - Fix the code
   - Re-run all test cases
   - Iterate until all pass

4. Once all examples pass, confirm with the user whether they want to test additional edge cases.

## Constraints Reminder

Before finalizing, verify:

- [ ] Uses Python ${python_version} compatible syntax only
- [ ] No imports outside the standard library
- [ ] No third-party packages
- [ ] Variable and function names are semantically meaningful
- [ ] Key algorithm steps have brief English comments
- [ ] All example test cases pass

## Important Notes
- The algorithm script should take its input from the standard input stream (for example, by reading `test_input.txt`) and write its output to the standard output stream.
- The current Python development environment is at a higher version than the one specified by ${python_version} and remains compatible with it; you simply need to ensure that the algorithm scripts use syntax supported by that ${python_version}.
