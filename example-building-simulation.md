# Example: Building a MythOS Simulation

Here’s a practical example of how to create and interact with a MythOS agent using Python. This snippet demonstrates the creation of a Product Manager agent in a startup simulation.

```python
from mythos import Agent, Simulation

# Initialize a simulation
sim = Simulation(scenario="Startup in Crisis")

# Create an agent
product_manager = Agent(
    role="Product Manager",
    traits=["analytical", "conflict-avoidant"],
    goals=["improve team morale", "launch new feature"]
)

# Agent observes the environment
context = product_manager.observe_environment()
print(context)
# Output: "Team morale is low. Resources are limited. Deadline approaching."

# Agent communicates with the CEO
response = product_manager.speak_to(agent="CEO", message="Propose team-building event to boost morale.")
print(response)
# Output: "CEO: Approved, but keep costs under $500."

# Agent adapts strategy based on feedback
product_manager.modify_strategy(new_priority="cost-effective morale boost")
```
