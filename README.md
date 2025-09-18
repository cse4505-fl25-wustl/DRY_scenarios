# DRY Principle Scenarios

This directory contains scenarios for learning the DRY (Don't Repeat Yourself) principle.

## Scenarios Overview

- [Scenario 1: Database Queries](./scenario_01_database_queries/scenario.md)
- [Scenario 2: Configuration Values](./scenario_02_configuration_values/scenario.md)
- [Scenario 3: Error Messages](./scenario_03_error_messages/scenario.md)
- [Scenario 4: Business Logic](./scenario_04_business_logic/scenario.md)
- [Scenario 5: Utility Functions](./scenario_05_utility_functions/scenario.md)
- [Scenario 6: UI Components](./scenario_06_ui_components/scenario.md)
- [Scenario 7: Data Transformation](./scenario_07_data_transformation/scenario.md)
- [Scenario 8: Constants](./scenario_08_constants/scenario.md)
- [Scenario 9: Input Sanitization](./scenario_09_input_sanitization/scenario.md)
- [Scenario 10: Logging](./scenario_10_logging/scenario.md)

## Key Questions to Consider

1. **Ask "What knowledge is duplicated?"** - Not just "Is the code similar?"

2. **Consider the rate of change** - Do these pieces need to change together?

3. **Think about purpose** - Similar code serving different purposes might be acceptable

4. **Watch for business rules** - These should almost always be centralized

5. **Configuration and constants** - Usually should be shared unless they represent genuinely different concepts

6. **When in doubt** - Lean toward DRY, but don't force inappropriate abstractions

**Remember:** Premature abstraction can be worse than duplication. Sometimes it's better to wait until you have 2+ instances before abstracting!
