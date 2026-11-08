# Lean Product Principles for Tuti

Tuti is being developed from observed needs in hospitality operations. We want a product that is useful, understandable, reliable, and economical to operate.

## What "lean" means to us

Lean does not mean cutting corners on correctness, privacy, or safety. It means avoiding unnecessary complexity and spending effort where it produces measurable user value.

1. **Solve a real workflow problem.** Start from an observed need, not a feature list.
2. **Prefer the smallest useful capability.** Build the simplest version that can be evaluated honestly.
3. **Measure before expanding.** Define expected behavior and test cases before adding complexity.
4. **Reuse before rebuilding.** Audit existing components and preserve working code where possible.
5. **Separate experiments from production.** Keep prototypes isolated until they pass review.
6. **Make uncertainty explicit.** A system should say when it lacks evidence.
7. **Control operating costs.** Prefer local, free-tier, or low-cost options when they meet the requirement; measure usage and set limits before enabling paid services.
8. **Protect people and data.** Use synthetic examples in public research and minimize personal data.
9. **Keep the interface simple.** Reduce visual clutter and make the next action obvious.
10. **Invite collaboration.** Publish questions, methods, and sanitized findings so others can challenge and improve the work.

## How we decide whether to add a feature

Before implementation, ask:
- Which user problem does it solve?
- What is the smallest testable version?
- How will we know it works?
- What new operational or security burden does it introduce?
- What does it cost to run and maintain?
- Can an existing component do the job with a small, safe change?

A feature is not a success merely because it has been implemented. It must improve a real workflow without creating disproportionate complexity.
