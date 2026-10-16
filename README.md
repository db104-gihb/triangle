# triangle

# Triangle Classifier

## Project Description

This Python program classifies triangles based on three
side lengths. It determines whether a triangle is valid
and classifies it as Equilateral, Isosceles, or Scalene.

The program also identifies right triangles.

## How to Run the Tests

1. Download or clone the GitHub repository.
2. Open the project folder in VS Code.
3. Open the terminal.
4. Install the required dependencies:

   python -m pip install -r requirements.txt

5. Run all tests:

   python -m pytest -v

## Equivalence Classes and Boundaries

Equivalence classes:

- Invalid: One or more sides are zero or negative.
- Invalid: The triangle inequality is not satisfied.
- Equilateral: All three sides are equal.
- Isosceles: Exactly two sides are equal.
- Scalene: All three sides are different.
- Right Triangle: The side lengths satisfy the
  Pythagorean theorem within a tolerance.

Boundary cases:

- A side length equal to zero.
- A negative side length.
- The sum of two sides exactly equals the third.
- The sum of two sides is slightly greater than
  the third.
- Non-integer sides forming a right triangle.

## Why Equilateral Triangles Cannot Be Right

An equilateral triangle has three equal angles of
60 degrees. A right triangle must contain a
90-degree angle, so it cannot be equilateral.

## Copilot Review Log

| Test | Copilot-suggested? | Decision | Why |
|------|--------------------|----------|-----|
| [Actual test name] | Yes/No | Kept/Edited/Rejected | [What you checked] |
| [Actual test name] | Yes/No | Kept/Edited/Rejected | [What you checked] |
| [Actual test name] | Yes/No | Kept/Edited/Rejected | [What you checked] |

## Acceptance Criteria

1. [Insert your first acceptance criterion.]
2. [Insert your second acceptance criterion.]
3. [Optional third acceptance criterion.]

## AI-Use Disclosure

GitHub Copilot was used to help draft unit tests
for Part 2. Suggestions were reviewed against
the assignment requirements before being accepted
or modified.

Part 3 acceptance criteria and acceptance testing
were completed without GitHub Copilot.

[Disclose any other AI tools actually used,
including ChatGPT, and what you verified.]
