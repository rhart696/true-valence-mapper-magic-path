# True Valence Relationship Mapper (Magic-Path Edition)

**Short name:** True Valence Mapper
**Edition type:** Methodology/Custom Framework
**Status:** 🚧 In Development

## Edition Focus

This edition implements the **Magic-Path** methodology - an intuitive, workflow-driven approach to relationship mapping that emphasizes user experience and natural interaction patterns.

## About Magic-Path

**Magic-Path** is a custom methodology designed specifically for True Valence Mapper that creates "magical" user experiences through:

- **Intuitive Workflows**: Minimize cognitive load with natural interaction patterns
- **Progressive Disclosure**: Reveal complexity only when needed
- **Contextual Guidance**: Smart suggestions based on user intent
- **Visual Clarity**: Clear visual representation of relationship paths

### Core Principles

1. **Simplicity First**: Start simple, add complexity only when valuable
2. **Path-Based Thinking**: Relationships as connected paths, not isolated nodes
3. **Contextual Intelligence**: System learns from user patterns
4. **Visual Storytelling**: Relationships tell stories through visual paths

## Key Features

### 1. Smart Path Detection
Automatically identifies common relationship patterns and suggests connections.

### 2. Visual Path Mapping
Beautiful, intuitive visual representation of relationship chains:
- Person → Organization → Project → Outcome

### 3. Contextual Recommendations
AI-powered suggestions based on:
- Similar relationship patterns
- Historical mapping data
- Domain-specific knowledge

### 4. Interactive Path Exploration
Navigate relationship networks interactively:
- Click to explore connections
- Hover for context
- Filter by relationship type
- Time-based path visualization

## Integration with True Valence Mapper

Magic-Path serves as the UX/CX layer for relationship mapping:

1. **User Interface**: Intuitive mapping interface with drag-and-drop
2. **Workflow Engine**: Guided workflows for common mapping scenarios
3. **Visualization**: Beautiful, interactive relationship visualizations
4. **Intelligence Layer**: AI-powered path suggestions and validations

## Architecture

```
magic-path/
├── workflows/              # Guided mapping workflows
│   ├── person-org.js      # Person-Organization mapping
│   ├── project-team.js    # Project-Team mapping
│   └── impact-chain.js    # Impact chain mapping
├── visualizations/         # Visual components
│   ├── path-viewer.jsx    # Interactive path viewer
│   ├── node-graph.jsx     # Network graph component
│   └── timeline.jsx       # Temporal relationship view
├── intelligence/           # AI-powered features
│   ├── pattern-detector.js # Detect relationship patterns
│   ├── recommender.js     # Suggest connections
│   └── validator.js       # Validate relationship logic
└── ux/                    # UX patterns and components
    ├── drag-drop.js       # Drag-drop interactions
    ├── contextual-menu.js # Context-aware menus
    └── onboarding.js      # User onboarding flows
```

## Usage Examples

### Create a Relationship Path

```javascript
// Intuitive API for creating relationship paths
const path = magicPath
  .start('person', 'Alice Smith')
  .connectTo('organization', 'Acme Corp', { role: 'CEO' })
  .connectTo('project', 'Product Launch', { involvement: 'sponsor' })
  .connectTo('outcome', 'Revenue Growth', { attribution: 0.8 })
  .build();

// Visualize the path
path.visualize({
  layout: 'timeline',
  interactive: true,
  showContext: true
});
```

### Smart Suggestions

```javascript
// Get AI-powered suggestions for next connection
const suggestions = await magicPath
  .from('Alice Smith')
  .suggestNextConnection({
    context: 'professional',
    limit: 5
  });

// suggestions: [
//   { type: 'organization', name: 'Tech Startup Inc', confidence: 0.92 },
//   { type: 'person', name: 'Bob Johnson', confidence: 0.87, relationship: 'colleague' },
//   ...
// ]
```

### Interactive Exploration

```javascript
// Enable interactive path exploration
magicPath.explore({
  startNode: 'Alice Smith',
  maxDepth: 3,
  filters: {
    relationshipTypes: ['employment', 'collaboration'],
    timeRange: { start: '2020-01-01', end: '2025-12-31' }
  },
  visualization: 'network-graph'
});
```

## Development Roadmap

### Phase 1: Foundation (Current)
- ✅ Core architecture design
- 🚧 Basic path creation API
- 🚧 Simple visualization components
- ⏳ Pattern detection engine

### Phase 2: Intelligence
- ⏳ AI-powered recommendations
- ⏳ Contextual suggestions
- ⏳ Automated validation
- ⏳ Learning from user behavior

### Phase 3: Advanced Features
- ⏳ Real-time collaboration
- ⏳ Time-travel (historical views)
- ⏳ Advanced analytics
- ⏳ Export/import capabilities

## Technology Stack

- **Frontend**: React, D3.js, Three.js (for 3D visualizations)
- **State Management**: Zustand or Jotai
- **Visualization**: D3.js, React Flow
- **AI Integration**: Claude Code API, pattern recognition
- **Backend**: Node.js (future), serverless functions

## Contributing

Magic-Path is a custom methodology developed for True Valence Mapper. Contributions should focus on:

1. **UX Improvements**: Making interactions more intuitive
2. **Visualization Enhancements**: Better ways to represent relationships
3. **Intelligence Features**: Smarter suggestions and validations
4. **Performance**: Faster rendering and interactions

## License

This edition follows the license of the True Valence Mapper project.

---

**Parent Repository**: [true-valence-mapper](https://github.com/rhart696/true-valence-mapper)
**Edition Status**: Custom Methodology
**Last Updated**: 2025-11-18
