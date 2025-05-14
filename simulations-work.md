# How MythOS Simulations Work

MythOS simulations are dynamic, agent-driven environments where interactions unfold organically within rule-based constraints. Here’s how the system operates:

## Dynamic Memory System

Unlike traditional AI systems that rely on static prompts, MythOS agents retrieve context just-in-time from the Memory Server. This ensures efficient, scalable simulations. Key features include:

- **Semantic Memory**: Agents store and query memories as vector embeddings, allowing for nuanced, context-aware recall.
- **Emotional Tagging**: Memories can be tagged with emotional states (e.g., "stressful meeting"), influencing future decisions.
- **Reflection and Belief Revision**: Agents periodically reflect on their experiences, updating their goals or strategies based on new insights.

Example: An agent who repeatedly fails to secure funding might tag those memories as "frustrating," prompting a shift toward more conservative financial strategies.

## Scenario Framework

MythOS provides a flexible framework for defining simulation scenarios. Each scenario includes:

- **Agent Roles**: Predefined or custom roles (e.g., CEO, Investor, Engineer).
- **MCP Tools**: The set of actions available to agents.
- **Social Protocols**: Rules governing interactions, such as communication hierarchies or decision-making authority.
- **Environmental Conditions**: Initial conditions, such as resource availability or external pressures.

Example Scenario: **"Startup in Crisis"**

- **Setup**: Agents are assigned roles (CEO, CFO, Product Manager, Investor). The environment simulates a cash-strapped startup facing a market downturn.
- **Interactions**: The CEO uses `speak_to(CFO)` to discuss cost-cutting, while the Product Manager uses `observe_environment()` to monitor team morale.
- **Outcome**: Agents negotiate, adapt strategies, and either stabilize the startup or fail, revealing insights about leadership and resilience.
