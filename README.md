# taalf-runtime
TAALF (Trigger–Assess–Align–Legitimize–Feedback) governance workflow runtime.

This project provides an abstract, auditable workflow for handling change under uncertainty.
It is not a decision-making AI, but a governance runtime that ensures decisions can be
explained, reviewed, and revisited later.

## Philosophy

TAALF does not decide what is correct.  
It ensures that change is handled in a way that can be explained later.

## License

Apache-2.0

## Usage

```python
from taalf.engine import TAALFEngine

engine = TAALFEngine()

result = engine.run(
    delta_s="価格改定の相談",
    domain="sales",
    scope="cross",
    inertia="high"
)

print(result)
