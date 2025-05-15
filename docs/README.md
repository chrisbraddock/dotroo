# Roo Documentation

This directory contains documentation for the Roo custom modes and workflows used in the MCP Ecosystem. This README provides an overview of the documentation structure, naming conventions, and guidelines for maintaining and extending the documentation.

## Key Concepts

### Custom Modes, Agents, and Human Roles

In our design system, we consider "custom modes" to be the explicit equivalent of "agents" in terms of AI agentic behavior. We also consider AI agents as (often) the AI analog of humans given a role. This conceptual framework allows us to:

1. Design workflows that mirror human team interactions
2. Create specialized AI agents with well-defined responsibilities
3. Establish clear handoff protocols between different specialized agents
4. Maintain a consistent mental model across human and AI collaborations

This equivalence (custom modes = agents = human role analogs) is fundamental to understanding our documentation and implementation approach.

## Directory Structure

The `.roo/docs` directory is organized as follows:

```
.roo/docs/
├── README.md                                 # This file
├── guide-mode-mapping-v1.2.0.md              # Reference guide for mode mapping
├── guide-integrated-modes-workflow-v1.2.0.md # Guide for workflow patterns
└── spec-custom-modes-implementation-v1.2.0.md # Technical specification
```

### Future Subdirectories

As the documentation grows, consider organizing it into the following subdirectories:

```
.roo/docs/
├── README.md
├── guides/        # User-focused how-to guides and reference documentation
├── specs/         # Technical specifications and implementation details
├── playbooks/     # Step-by-step procedures for common tasks
└── examples/      # Example configurations and use cases
```

## Documentation Types

The documentation follows a structured approach with different document types serving specific purposes:

1. **Guides (`guide-*.md`)**: User-focused documentation that explains how to use features, provides reference information, and offers best practices. Guides answer "how to" questions.

2. **Specifications (`spec-*.md`)**: Technical documentation that details the implementation, architecture, and design decisions. Specifications answer "how it works" questions.

3. **Playbooks (`playbook-*.md`)**: Step-by-step procedures for accomplishing specific tasks or workflows. Playbooks answer "what steps to follow" questions.

4. **Analysis (`analysis-*.md`)**: In-depth examination of problems, requirements, or existing systems. Analysis documents answer "what and why" questions.

5. **Plans (`plan-*.md`)**: Forward-looking documents outlining future work, roadmaps, or implementation strategies. Plans answer "what will be done" questions.

## Naming Conventions

All documentation follows this naming convention:

```
[document-type]-[descriptive-name]-v[major].[minor].[patch].[extension]
```

Where:
- **document-type**: The type of document (guide, spec, playbook, analysis, plan)
- **descriptive-name**: A hyphen-separated name describing the content
- **version**: Semantic versioning with major.minor.patch format
- **extension**: File extension (typically .md for Markdown)

Examples:
- `guide-mode-mapping-v1.2.0.md`
- `spec-custom-modes-implementation-v1.2.0.md`
- `playbook-settings-synchronization-v1.0.0.md`

## Versioning Guidelines

When updating documentation:

1. **Patch Version (v1.0.x)**: Increment for minor corrections, typo fixes, or clarifications that don't change the content's meaning.

2. **Minor Version (v1.x.0)**: Increment for additions, improvements, or restructuring that doesn't fundamentally change the document's purpose or main content.

3. **Major Version (vx.0.0)**: Increment for significant rewrites, changes to the document's purpose, or when the subject matter itself has undergone major changes.

## Current Documentation

### Mode Mapping Guide

**File**: `guide-mode-mapping-v1.2.0.md`

This guide provides a mapping between Roo's built-in modes and their industry-standard equivalents. It includes:
- Built-in mode to industry-standard role mapping
- Additional custom modes
- Mode selection guidelines
- Mode transition guidelines
- Implementation details

### Integrated Modes Workflow Guide

**File**: `guide-integrated-modes-workflow-v1.2.0.md`

This guide outlines the detailed role definitions and workflow diagrams for our integrated mode ecosystem. It includes:
- Role definitions for built-in and custom modes
- Workflow diagrams for common scenarios
- Integration points between modes
- Implementation steps
- Success metrics

### Custom Modes Implementation Specification

**File**: `spec-custom-modes-implementation-v1.2.0.md`

This specification details the implementation of our custom modes ecosystem. It includes:
- Overall architecture
- Mode implementations with JSON configurations
- Workflow patterns
- Implementation steps
- Success metrics

## Documentation Standards

When creating or updating documentation:

1. **Use Clear Headings**: Organize content with descriptive headings and subheadings.

2. **Include Examples**: Provide examples to illustrate concepts where appropriate.

3. **Use Diagrams**: Include diagrams (Mermaid, PlantUML, etc.) for complex workflows or architectures.

4. **Cross-Reference**: Link to related documentation using relative paths.

5. **Maintain Consistency**: Use consistent terminology, formatting, and structure across documents.

6. **Consider the Audience**: Adjust technical depth based on the intended audience.

7. **Include Tables of Contents**: For longer documents, include a table of contents.

8. **Use Markdown Effectively**: Leverage Markdown formatting for readability.

## Contributing to Documentation

When contributing to the documentation:

1. **Follow Naming Conventions**: Use the established naming convention for new files.

2. **Update the README**: Add new documents to this README when created.

3. **Update Cross-References**: Ensure cross-references are updated when files are renamed or moved.

4. **Increment Versions**: Follow the versioning guidelines when updating documents.

5. **Maintain Structure**: Place new documents in the appropriate directory based on their type.

6. **Review Existing Docs**: Familiarize yourself with existing documentation to maintain consistency.

7. **Test Links**: Ensure all links work correctly before committing changes.