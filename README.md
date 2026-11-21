# Rubric Review Examples

Examples of how I review AI evaluation rubrics for fairness, clarity, and consistency.

I focus on: one check per criterion, accepting all valid answers, and separating reasoning from the check itself.

## Example 1: Bounding-Box Annotation

Task: Draw a box around each tool in an image.

Common mistake: Grouping several tools in one big box.

My rule: One object = one box. Box must be tight to the edges. Ignore scattered items that are not part of the target list.

## Example 2: Rubric Clarity

Flawed criterion:
> Places an order with the correct vegetarian dish.

Why it's flawed:
It only accepts one dish when the prompt allows any vegetarian dish. It also mixes reasoning into the criterion.

Better version:
> Places an order with at least 2 vegetarian entrees.

Explanation: Prompt says 2 people are vegetarian.

## My Review Checklist

1. Does each criterion check only ONE thing?
2. Does it start with Places... or Charges...?
3. Does it accept every value the prompt allows (use "or")?
4. Is the delivery time written as "in a delivery window that includes [time]"?
5. If instructions conflict, does the newest one win?
6. Is reasoning in the Explanation, not in the criterion?
