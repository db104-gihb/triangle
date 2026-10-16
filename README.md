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
| test_equilateral_triangle | Yes | Kept | Verified that three equal sides return "Equilateral" as required. |
| test_invalid_triangle | Yes | Edited | Checked that zero, negative, and invalid side lengths return "Invalid" without errors. |
| test_right_triangle | Yes | Edited | Checked that the test uses non-integer side lengths to verify right-triangle detection with a numerical tolerance instead of exact equality. |
## Acceptance Criteria

1. **Triangle Validation:** When a customer enters three side lengths, the system must correctly identify whether they form a valid triangle. If any side is zero or negative, or the sum of two sides is less than or equal to the third, the system must return "Invalid" without crashing.

2. **Triangle Classification:** When a customer enters three valid side lengths, the system must correctly classify the triangle as "Equilateral," "Isosceles," or "Scalene" based on the lengths of its sides.

3. **Right Triangle Detection:** When a customer enters side lengths that satisfy the Pythagorean theorem within a numerical tolerance, the system must identify the triangle as a right triangle by adding "Right" before its classification, such as "Right Scalene."
## AI-Use Disclosure

GitHub Copilot was used to help draft unit tests
for Part 2. Suggestions were reviewed against
the assignment requirements before being accepted
or modified.

Part 3 acceptance criteria and acceptance testing
were completed without GitHub Copilot.

[Disclose any other AI tools actually used,
including ChatGPT, and what you verified.]
