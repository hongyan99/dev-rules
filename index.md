# Software Development Lifecycle Rules

This directory contains focused rule sets for different phases of the software development lifecycle. Each file provides specific guidance relevant to that particular phase or activity.

## Development Lifecycle Phases

1. **Requirements Analysis** → [requirements_analysis_rules.md](requirements_analysis_rules.md)
   - Gathering and analyzing user needs
   - Defining project scope and constraints
   - Creating functional and non-functional requirements

2. **Design** → [design_phase_rules.md](design_phase_rules.md)
   - System architecture
   - Component interfaces and contracts
   - Data modeling

3. **Implementation** → [implementation_phase_rules.md](implementation_phase_rules.md)
   - Writing code that fulfills design specifications
   - Following coding standards
   - Unit testing

4. **Testing** → [testing_rules.md](testing_rules.md)
   - Developing test plans and test cases
   - Performing integration and system testing
   - Validating requirements

5. **Deployment** → [deployment_rules.md](deployment_rules.md)
   - Moving software to production environment
   - Configuration management
   - Rollout strategies

6. **Maintenance** → [maintenance_phase_rules.md](maintenance_phase_rules.md)
   - Bug fixes and minor enhancements
   - Managing technical debt
   - Incremental refactoring

## Cross-cutting Concerns

1. **Performance Optimization** → [performance_optimization_rules.md](performance_optimization_rules.md)
   - Identifying and resolving bottlenecks
   - Improving resource usage
   - Measuring and monitoring performance

2. **Security** → [security_rules.md](security_rules.md)
   - Implementing security controls
   - Vulnerability assessment
   - Secure coding practices

3. **Documentation** → [documentation_rules.md](documentation_rules.md)
   - Code documentation
   - Technical documentation
   - User documentation

4. **Knowledge Graph** → [knowledge_graph_rules.md](knowledge_graph_rules.md)
   - Maintaining project context across sessions
   - Standardized entity and relation types
   - Knowledge Graph usage guidelines

5. **Cross-Phase Practices** → [cross_phase_practices.md](cross_phase_practices.md)
   - Practices that span multiple development phases
   - Continuous activities throughout the lifecycle
   - Bridging between different development stages

## Learning and Improvement

1. **Lessons Learned** → [lessons_learned.md](lessons_learned.md)
   - Record of past mistakes and their impact
   - Specific lessons extracted from experience
   - Continuously updated as new lessons are learned

## Using These Rules

- Refer to the appropriate rule file for your current development phase
- Many practices overlap between phases - see [cross_phase_practices.md](cross_phase_practices.md)
- Some rules apply to multiple phases (noted in each file)
- Critical rules are marked with **NEVER** or **ALWAYS** for emphasis
- Consider creating a project-specific checklist based on these rules
- Adapt these rules to your project's specific context and constraints
- Review [lessons_learned.md](lessons_learned.md) periodically to avoid repeating past mistakes

## Maintaining These Rules

- Focus on consolidating and refining existing rules rather than just adding new ones
- When a new lesson is learned, first check if an existing rule can be enhanced
- Periodically review all rules for relevance, clarity, and consistency
- Remove or archive outdated rules to prevent rule bloat
- Maintain a reasonable number of rules to ensure they remain practical to follow
- Test rules by applying them to past mistakes to verify they would have prevented the issue