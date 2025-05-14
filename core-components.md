# Core Components of MythOS

MythOS is built around three foundational pillars: self-evolving AI agents, MCP-powered actions, and modular MCP servers. Together, these components create a robust framework for simulating complex systems.

## Self-Evolving AI Agents

At the heart of MythOS are its AI agents—autonomous entities that go beyond scripted responses to exhibit adaptive, human-like behavior. Key features include:

- **Lightweight Initialization**: Agents are created from simple prompts that define their role, personality, and goals. For example:
  ```
  "Optimistic engineer, risk-tolerant, focused on rapid prototyping"
  ```
- **Recursive Reasoning**: Agents use iterative thinking to process information, make decisions, and adapt their strategies based on new data.
- **Dynamic Evolution**: Through interactions and reflection, agents can modify their internal states, goals, or even personality traits over time.
- **Memory-Driven Behavior**: Agents leverage a long-term memory system to recall past events, relationships, and lessons, ensuring contextually relevant actions.

Example: An agent initialized as a cautious CFO might become more risk-tolerant after repeated successful collaborations with a bold CEO, reflecting real-world learning.

## MCP-Powered Actions

Every MythOS agent is equipped with a suite of tools defined by the Model-Context-Protocol (MCP) standard. These tools allow agents to interact with their environment and other agents in structured, traceable ways. Core MCP actions include:

- `observe_environment()`: Collects data about the simulation world, such as nearby agents, objects, or events.
- `speak_to(agent)`: Facilitates structured communication with other agents, adhering to social protocols.
- `search_memory()`: Retrieves relevant information from the agent’s personal or shared memory (stored in a vector database).
- `move(location)`: Enables location-based actions within the simulation’s spatial environment.
- `modify_strategy()`: Allows the agent to adapt its goals, priorities, or behavior based on new insights.

Example: In a simulated startup, an agent (Product Manager) might use `observe_environment()` to detect a drop in team morale, then call `speak_to(CEO)` to propose a morale-boosting initiative.

## Modular MCP Servers

MythOS environments are powered by a collection of MCP servers, each handling a specific aspect of the simulation. These servers ensure modularity, scalability, and flexibility. The core servers are:

- **Environment Server**: Manages the physical and spatial aspects of the simulation, such as locations, objects, and environmental changes.
- **Memory Server**: Stores and retrieves long-term memory for agents using a vector database, supporting semantic search and context-aware recall.
- **Comms Server**: Routes structured communications between agents, ensuring messages adhere to defined protocols.
- **Protocol Server**: Defines and enforces social norms, hierarchies, and rules that govern agent interactions (e.g., who can speak to whom, under what conditions).
- **Knowledge Server (optional)**: Provides background information, domain-specific rules, or "lore" to enrich the simulation.

Example: In a crisis simulation, the Protocol Server might enforce a rule where only senior agents can make binding decisions, while the Environment Server simulates a declining resource pool.
