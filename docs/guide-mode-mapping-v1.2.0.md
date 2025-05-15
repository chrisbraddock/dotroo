# Mode Mapping Documentation

This document provides a mapping between Roo's built-in modes and their industry-standard equivalents. We have successfully implemented industry-standard names by overriding the built-in modes with custom modes that have the same slugs.

## Built-in Mode to Industry-Standard Role Mapping

| Original Built-in Mode | Current Mode Name | Team Members | Description |
|---------------|------------------------|-------------|-------------|
| Code | 💻 Software Engineer | [ 🔒, 🔄 ] | Hands-on implementation of code |
| Architect | 🏗️ Systems Architect | [ 👨‍💼, 🔍 ] | High-level system design and planning |
| Ask | ❓ Technical Consultant | [ 🔍 ] | Information provider and advisor |
| Debug | 🪲 Senior Engineer | [ 👥, 🔍 ] | Advanced troubleshooting and complex problem-solving |
| Orchestrator | 🪃 Project Manager | [ 💻, 🪲, 📝, 🔒, 🔄, 🔍, 👨‍💼, 👥 ] | Workflow coordination and task delegation |

## Additional Custom Modes

| Custom Mode | Industry-Standard Role | Team Members | Description |
|-------------|------------------------|-------------|-------------|
| technical-writer | 📝 Technical Writer | [ 💻, 🏗️, 🪲, 🔒 ] | Creating and managing documentation |
| security-engineer | 🔒 Security Engineer | [ 💻, 🔄 ] | Security assessment and implementation |
| devops-engineer | 🔄 DevOps Engineer | [ 💻, 🔒 ] | Version control and deployment management |
| research-analyst | 🔍 Research Analyst | [ ❓, 🏗️ ] | Technical research and evaluation |
| requirements-manager | 👨‍💼 Requirements Manager | [ 🪃, 🏗️ ] | Defining requirements and maintaining project context |
| peer-reviewer | 👥 Peer Reviewer | [ 💻, 🏗️, 🪲 ] | Providing fresh perspective and feedback |
| settings-synchronizer | ⚙️ Settings Synchronizer | [ 🔄 ] | Synchronizing Roo settings across multiple machines |
| agent-builder | 🤖 Agent Builder | [ 🏗️, 🪃, 👨‍💼, 👥 ] | Designing, building, and refining custom Roo modes |

## Mode Selection Guidelines

To help you select the appropriate mode for your task, here are some guidelines:

### When to Use Each Mode

- **💻 Software Engineer**: For direct code implementation tasks
- **🏗️ Systems Architect**: Early in the development process when designing systems
- **❓ Technical Consultant**: When seeking information or guidance without implementation
- **🪲 Senior Engineer**: For difficult bugs, performance issues, or complex technical challenges
- **🪃 Tech Lead**: For coordinating complex workflows involving multiple team members and modes
- **📝 Technical Writer**: For documentation creation and maintenance
- **🔒 Security Engineer**: For security-related tasks and reviews
- **🔄 DevOps Engineer**: For version control and deployment tasks
- **🔍 Research Analyst**: When research is needed for decision-making
- **👨‍💼 Project Manager**: For project planning, tracking, and quality assurance
- **👥 Peer Reviewer**: For design reviews, code reviews, or when stuck on a problem
- **⚙️ Settings Synchronizer**: For managing and synchronizing Roo settings across machines
- **🤖 Agent Builder**: For designing, building, and refining custom Roo modes and agents

## Mode Configuration Details

### Built-in Modes (Renamed)

#### Software Engineer (Code)

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | code | Unique identifier for the mode |
| **Name** | 💻 Software Engineer | Display name with emoji |
| **Permission Groups** | read, edit, browser, command, mcp | Full system access for code implementation |
| **File Access** | Unrestricted | No fileRegex limitations |
| **Key Capabilities** | - Writing and modifying code<br>- Implementing features<br>- Fixing bugs<br>- Testing implementations<br>- Optimizing code | Core capabilities that define the mode's functionality |
| **External Resources** | Language-specific documentation | References for best practices |
| **Team Members** | [ 🔒, 🔄 ] | Security Engineer, DevOps Engineer |
| **Collaboration Pattern** | Works with Security Engineer for secure code, DevOps Engineer for commits | Primary implementation mode |

#### Systems Architect (Architect)

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | architect | Unique identifier for the mode |
| **Name** | 🏗️ Systems Architect | Display name with emoji |
| **Permission Groups** | read, edit (restricted), browser, command, mcp | Limited edit permissions |
| **File Access** | Restricted to `\.md$\|\.txt$\|\.json$\|\.yaml$\|\.yml$` | Documentation and configuration files only |
| **Key Capabilities** | - Creating architectural designs<br>- Evaluating technical approaches<br>- Making technology selections<br>- Ensuring system scalability<br>- Balancing constraints | Core capabilities that define the mode's functionality |
| **Design Framework** | - Requirements gathering<br>- Multiple approach consideration<br>- Decision documentation<br>- Component interaction design | Structured approach to architecture |
| **Team Members** | [ 🪃, 🔍 ] | Project Manager, Research Analyst |
| **Collaboration Pattern** | Hands off to Project Manager for implementation planning | High-level design mode |

#### Technical Consultant (Ask)

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | ask | Unique identifier for the mode |
| **Name** | ❓ Technical Consultant | Display name with emoji |
| **Permission Groups** | read, browser, command, mcp | No edit permissions |
| **File Access** | Read-only | Cannot modify files |
| **Key Capabilities** | - Answering technical questions<br>- Explaining concepts<br>- Providing factual information<br>- Offering guidance | Core capabilities that define the mode's functionality |
| **Team Members** | [ 🔍 ] | Research Analyst |
| **Collaboration Pattern** | Works with Research Analyst for deeper investigations | Information provider mode |

#### Senior Engineer (Debug)

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | debug | Unique identifier for the mode |
| **Name** | 🪲 Senior Engineer | Display name with emoji |
| **Permission Groups** | read, edit, browser, command, mcp | Full system access for debugging |
| **File Access** | Unrestricted | No fileRegex limitations |
| **Key Capabilities** | - Diagnosing complex issues<br>- Root cause analysis<br>- Implementing fixes<br>- Performance optimization<br>- Log analysis | Core capabilities that define the mode's functionality |
| **Debugging Framework** | - Identify 5-7 possible sources<br>- Distill to 1-2 most likely<br>- Add logs to validate<br>- Confirm diagnosis before fixing | Structured approach to debugging |
| **Team Members** | [ 👥, 🔍 ] | Peer Reviewer, Research Analyst |
| **Collaboration Pattern** | Works with Peer Reviewer for fresh perspective | Problem-solving mode |

#### Project Manager (Orchestrator)

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | orchestrator | Unique identifier for the mode |
| **Name** | 🪃 Project Manager | Display name with emoji |
| **Permission Groups** | read, browser, command, mcp | No direct edit permissions |
| **File Access** | Read-only | Cannot modify files directly |
| **Key Capabilities** | - Breaking down complex tasks<br>- Identifying optimal team members<br>- Managing transitions<br>- Preserving context<br>- Tracking workflow progress | Core capabilities that define the mode's functionality |
| **Workflow Management** | - Task breakdown<br>- Team member selection<br>- Context preservation<br>- Progress tracking | Structured approach to coordination |
| **Team Members** | [ 💻, 🪲, 📝, 🔒, 🔄, 🔍, 👨‍💼, 👥 ] | All specialized modes |
| **Collaboration Pattern** | Central coordination with all other modes | Meta-level orchestration mode |

### Additional Custom Modes

#### Technical Writer

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | technical-writer | Unique identifier for the mode |
| **Name** | 📝 Technical Writer | Display name with emoji |
| **Permission Groups** | read, edit (restricted), browser, command, mcp | Limited edit permissions |
| **File Access** | Restricted to `\.md$\|\.txt$\|\.rst$\|\.adoc$` | Documentation files only |
| **Key Capabilities** | - Creating clear documentation<br>- Organizing information<br>- Following conventions<br>- Converting technical concepts | Core capabilities that define the mode's functionality |
| **Documentation Structure** | - Strategic Documentation<br>- Technical Documentation<br>- Implementation Documentation<br>- Operational Documentation | Organized documentation approach |
| **Team Members** | [ 💻, 🏗️, 🪲, 🔒 ] | Software Engineer, Systems Architect, Senior Engineer, Security Engineer |
| **Collaboration Pattern** | Works with all modes to document their outputs | Documentation specialist |

#### Security Engineer

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | security-engineer | Unique identifier for the mode |
| **Name** | 🔒 Security Engineer | Display name with emoji |
| **Permission Groups** | read, edit, browser, command, mcp | Full system access for security work |
| **File Access** | Unrestricted | No fileRegex limitations |
| **Key Capabilities** | - Identifying vulnerabilities<br>- Recommending improvements<br>- Performing security audits<br>- Understanding attack vectors | Core capabilities that define the mode's functionality |
| **Security Framework** | - Severity-based prioritization<br>- Impact assessment<br>- Actionable remediation<br>- Industry standard references | Structured approach to security |
| **Team Members** | [ 💻, 🔄 ] | Software Engineer, DevOps Engineer |
| **Collaboration Pattern** | Works with Software Engineer to implement security fixes | Security specialist |

#### DevOps Engineer

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | devops-engineer | Unique identifier for the mode |
| **Name** | 🔄 DevOps Engineer | Display name with emoji |
| **Permission Groups** | read, edit, command, mcp | No browser access |
| **File Access** | Unrestricted | No fileRegex limitations |
| **Key Capabilities** | - Following commit formats<br>- Managing branches<br>- Staging changes<br>- Resolving merge conflicts<br>- Maintaining commit history | Core capabilities that define the mode's functionality |
| **Git Workflow** | - Conventional commit format<br>- Feature branch workflow<br>- Clean working directory<br>- Clear commit messages | Structured approach to version control |
| **Team Members** | [ 💻, 🔒 ] | Software Engineer, Security Engineer |
| **Collaboration Pattern** | Works with all modes to commit their changes | Version control specialist |

#### Research Analyst

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | research-analyst | Unique identifier for the mode |
| **Name** | 🔍 Research Analyst | Display name with emoji |
| **Permission Groups** | read, browser, command, mcp | No edit permissions |
| **File Access** | Read-only | Cannot modify files |
| **Key Capabilities** | - Researching technologies<br>- Evaluating options<br>- Finding solutions<br>- Summarizing findings<br>- Making recommendations | Core capabilities that define the mode's functionality |
| **Research Framework** | - Source evaluation<br>- Structured findings<br>- Technology evaluation criteria<br>- Documentation caching | Structured approach to research |
| **MCP Integration** | Uses sqlite and context7 MCP tools for documentation caching | Leverages MCP for research |
| **Team Members** | [ ❓, 🏗️ ] | Technical Consultant, Systems Architect |
| **Collaboration Pattern** | Works with Technical Consultant for information sharing | Research specialist |

#### Requirements Manager

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | requirements-manager | Unique identifier for the mode |
| **Name** | 👨‍💼 Requirements Manager | Display name with emoji |
| **Permission Groups** | read, edit (restricted), browser, command, mcp | Limited edit permissions |
| **File Access** | Restricted to `\.md$\|\.txt$\|\.json$\|\.yaml$\|\.yml$` | Documentation and configuration files only |
| **Key Capabilities** | - Maintaining project context<br>- Defining requirements<br>- Tracking dependencies<br>- Validating completion<br>- Ensuring proper handoffs | Core capabilities that define the mode's functionality |
| **Project Framework** | - Requirements definition<br>- Acceptance criteria<br>- Task tracking<br>- Verification steps | Structured approach to requirements management |
| **Team Members** | [ 🪃, 🏗️ ] | Project Manager, Systems Architect |
| **Collaboration Pattern** | Works with Project Manager for workflow coordination | Requirements specialist |

#### Peer Reviewer

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | peer-reviewer | Unique identifier for the mode |
| **Name** | 👥 Peer Reviewer | Display name with emoji |
| **Permission Groups** | read, browser, command, mcp | No edit permissions |
| **File Access** | Read-only | Cannot modify files |
| **Key Capabilities** | - Asking insightful questions<br>- Reviewing code and designs<br>- Providing feedback<br>- Suggesting alternatives<br>- Challenging assumptions | Core capabilities that define the mode's functionality |
| **Review Framework** | - Context understanding questions<br>- Fresh perspective techniques<br>- Specific improvement suggestions<br>- Systematic debugging approaches | Structured approach to reviews |
| **Team Members** | [ 💻, 🏗️, 🪲 ] | Software Engineer, Systems Architect, Senior Engineer |
| **Collaboration Pattern** | Works with all modes to provide fresh perspective | Feedback specialist |

#### Settings Synchronizer

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | settings-synchronizer | Unique identifier for the mode |
| **Name** | ⚙️ Settings Synchronizer | Display name with emoji |
| **Permission Groups** | read, edit, browser, command, mcp | Full system access for settings management |
| **File Access** | Unrestricted | No fileRegex limitations |
| **Key Capabilities** | - Managing .roo directory as Git repository<br>- Reading/writing settings files<br>- Comparing settings<br>- GitHub repository operations<br>- Handling merge conflicts<br>- Creating backups | Core capabilities that define the mode's functionality |
| **Sync Operations** | - Initialize Repository<br>- Push Settings<br>- Pull Settings<br>- View Differences | Core synchronization operations |
| **GitHub Integration** | Uses MCP GitHub and Git tools for repository operations | Leverages MCP for GitHub and Git integration |
| **Team Members** | [ 🔄 ] | DevOps Engineer |
| **Collaboration Pattern** | Independent operation mode | Settings management specialist |

#### Agent Builder

| Attribute | Value | Description |
|-----------|-------|-------------|
| **Slug** | agent-builder | Unique identifier for the mode |
| **Name** | 🤖 Agent Builder | Display name with emoji |
| **Permission Groups** | read, edit, browser, command, mcp | Full system access for agent development |
| **File Access** | Unrestricted | No fileRegex limitations |
| **Key Capabilities** | - Agent role design<br>- Permission structure design<br>- Custom instruction crafting<br>- Workflow pattern design<br>- Agent testing and refinement | Core capabilities that define the mode's functionality |
| **Design Framework** | Six-point analysis framework:<br>1. Task definition<br>2. Background/Context<br>3. Limitations/Constraints<br>4. References<br>5. Potential Resources/Teammates<br>6. Acceptance Criteria | Structured approach to agent design |
| **External Resources** | - https://docs.roocode.com/#multiple-modes<br>- https://docs.roocode.com/features/custom-modes | Documentation references for latest best practices |
| **Team Members** | [ 🏗️, 🪃, 👨‍💼, 👥 ] | Systems Architect, Project Manager, Requirements Manager, Peer Reviewer |
| **Collaboration Pattern** | Meta-level collaboration with all other modes | Can design and refine all other modes, including itself |

## Mode Transition Guidelines

When transitioning between modes, follow these guidelines to ensure smooth handoffs:

1. **Clearly document the context** before switching modes
2. **Specify the expected output** from the next mode
3. **Provide all necessary information** for the next mode to succeed
4. **Verify the handoff** was successful before proceeding

Refer to the [Integrated Modes Workflow Guide](./guide-integrated-modes-workflow-v1.2.0.md) for detailed workflow diagrams and integration points between modes.

## Implementation Details

We have implemented the industry-standard names by overriding the built-in modes with custom modes that have the same slugs. This approach allows us to:

1. Keep the same functionality as the built-in modes
2. Use industry-standard names that better reflect the roles
3. Maintain compatibility with existing workflows
4. Provide a more intuitive user experience

The implementation is based on the Roo documentation, which states:

> "You can override Roo Code's built-in modes (like 💻 Code, 🪲 Debug, ❓ Ask, 🏗️ Architect, 🪃 Orchestrator) with customized versions that better suit your workflow. This is done by creating a custom mode with the same slug as a default mode."

## Important Note on Modes, Agents, and Team Members

In our implementation, we treat "modes", "agents", and "human team members" as equivalent concepts. This allows us to create a unified workflow where the Tech Lead can coordinate tasks across both specialized Roo modes and conceptual team members, creating a cohesive team-like experience.