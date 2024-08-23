This script defines the creation of tables and the insertion of initial data for an organizational database structure, focusing on regions, countries, locations, jobs, departments, employees, and dependents. Below is a breakdown of the main elements:

## Table Creation:
1. **regions**: Stores region information with `region_id` as the primary key.
2. **countries**: Stores country information with `country_id` as the primary key and references `regions`.
3. **locations**: Stores location details, referencing `countries`.
4. **jobs**: Stores job roles with `job_id` as the primary key.
5. **departments**: Stores department information, referencing `locations`.
6. **employees**: Stores employee details, including references to jobs, departments, and managers (self-referencing).
7. **dependents**: Stores dependent information, referencing `employees`.

### Data Insertion:
- **regions**: Populates initial regions with specific IDs.
- **countries**: Inserts various countries associated with regions.
- **locations**: Adds location entries with references to countries.
- **jobs**: Inserts predefined job titles with salary ranges.
- **departments**: Adds departments linked to specific locations.
- **employees**: Populates employee records, including their hierarchy.
- **dependents**: Inserts dependent information linked to employees.

This setup enables a hierarchical structure of regions, countries, and locations, followed by departments and employees, reflecting a realistic organizational structure. The cascading delete and update operations ensure data integrity across related tables.
