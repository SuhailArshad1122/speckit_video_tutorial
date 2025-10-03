# Speckit Video Tutorial Constitution
<!-- Version: 1.0.0 -->
<!-- Last Amended: 2025-10-03 -->
<!-- 
Sync Impact Report:
- Version change: 0.0.0 → 1.0.0
- Added: Core principles for clean, modular code and Next.js 15 best practices
- Updated: All placeholders with concrete content
-->

## Core Principles

### I. Component-Driven Architecture
- Build UI using small, reusable components that do one thing well
- Follow the Single Responsibility Principle for all components
- Use the `app` directory structure for routing and layouts
- Implement Server Components by default, only use Client Components when necessary
- Colocate component tests with their respective components

### [PRINCIPLE_2_NAME]
<!-- Example: II. CLI Interface -->
[PRINCIPLE_2_DESCRIPTION]
<!-- Example: Every library exposes functionality via CLI; Text in/out protocol: stdin/args → stdout, errors → stderr; Support JSON + human-readable formats -->

### [PRINCIPLE_3_NAME]
<!-- Example: III. Test-First (NON-NEGOTIABLE) -->
[PRINCIPLE_3_DESCRIPTION]
<!-- Example: TDD mandatory: Tests written → User approved → Tests fail → Then implement; Red-Green-Refactor cycle strictly enforced -->

### [PRINCIPLE_4_NAME]
<!-- Example: IV. Integration Testing -->
[PRINCIPLE_4_DESCRIPTION]
<!-- Example: Focus areas requiring integration tests: New library contract tests, Contract changes, Inter-service communication, Shared schemas -->

### [PRINCIPLE_5_NAME]
<!-- Example: V. Observability, VI. Versioning & Breaking Changes, VII. Simplicity -->
[PRINCIPLE_5_DESCRIPTION]
<!-- Example: Text I/O ensures debuggability; Structured logging required; Or: MAJOR.MINOR.BUILD format; Or: Start simple, YAGNI principles -->

## [SECTION_2_NAME]
<!-- Example: Additional Constraints, Security Requirements, Performance Standards, etc. -->

[SECTION_2_CONTENT]
<!-- Example: Technology stack requirements, compliance standards, deployment policies, etc. -->

## [SECTION_3_NAME]
<!-- Example: Development Workflow, Review Process, Quality Gates, etc. -->

<!-- Example: Code review requirements, testing gates, deployment approval process, etc. -->

## Governance
<!-- Example: Constitution supersedes all other practices; Amendments require documentation, approval, migration plan -->

### II. Type Safety First
- Use TypeScript for all new code
- Define strict types for all props, API responses, and state
- Use Zod for runtime validation of external data
- Avoid `any` type - prefer explicit types or `unknown` with type guards
- Document complex types with JSDoc comments

### III. Performance Optimization
- Implement code splitting using dynamic imports for large components
- Optimize images using Next.js Image component
- Use React.memo, useMemo, and useCallback appropriately
- Implement proper loading states and error boundaries
- Follow Next.js 15's partial rendering and streaming recommendations

### IV. State Management
- Prefer React Server Components and server actions for data fetching
- Use React Context for shared client state when needed
- Consider Zustand or Jotai for complex client state
- Keep state as local as possible to the components that need it
- Normalize state shape to avoid duplication

### V. Code Organization
- Follow the Next.js 13+ app directory structure
- Group by feature, not by file type
- Use barrel files (index.ts) for clean imports
- Keep utility functions in dedicated files
- Maintain a consistent folder structure across the project

## Governance

### Versioning
- Current Version: 1.0.0
- Ratified: 2025-10-03
- Last Amended: 2025-10-03

### Amendment Process
1. Propose changes via Pull Request
2. Require at least one code review approval
3. Update version number following semantic versioning
4. Update the Last Amended date
5. Document changes in the Sync Impact Report comment

### Compliance
- All new code must pass TypeScript and ESLint checks
- CI/CD pipeline enforces code quality gates
- Regular code reviews required
- Document any deviations with justification