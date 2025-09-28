# Planning Structure

This folder uses a hierarchical time-based planning system optimized for easy AI navigation and automatic date-based organization.

## Folder Structure

```
planning/
└── {YEAR}/                         # e.g., 2025/
    └── {MM-month}/                 # e.g., 07-july/
        ├── month_plan.md           # Monthly overview and themes
        └── week-{YYYY-MM-DD}/      # e.g., week-2025-07-28/ (Monday of that week)
            ├── week_plan.md        # Weekly focus and objectives
            └── day_{DD}.md         # e.g., day_29.md, day_30.md, day_31.md
```

## Date-Based Week Naming

Week folders use the **Monday date** of that week for consistent, AI-friendly navigation:
- `week-2025-07-07/` = Week starting Monday, July 7th
- `week-2025-07-14/` = Week starting Monday, July 14th
- `week-2025-07-28/` = Week starting Monday, July 28th

This eliminates complex "week number" calculations and makes it easy for AI to find the correct week folder.

## Navigation Examples

- **Today's plan**: `planning/2025/07-july/week-2025-07-28/day_29.md`
- **This week's plan**: `planning/2025/07-july/week-2025-07-28/week_plan.md`
- **This month's plan**: `planning/2025/07-july/month_plan.md`

## AI Navigation Logic

For AI assistants to find the correct week folder:
1. **Take any date** (e.g., July 29, 2025)
2. **Find the Monday** of that week (July 28, 2025)
3. **Look for folder** `week-2025-07-28/`
4. **If not found**, create it using the Monday date format

## Creating New Structure

### New Month
1. Create folder: `planning/2025/08-august/`
2. Create file: `month_plan.md`
3. Week folders will be created as needed using Monday dates

### New Week
1. Navigate to month folder: `planning/2025/08-august/`
2. Calculate Monday of the target week
3. Create folder: `week-2025-08-05/` (using Monday date)
4. Create file: `week_plan.md`
5. Create daily files as needed: `day_05.md`, `day_06.md`, etc.

### Week Folder Creation Examples
- For any date in the week of August 5-11: create `week-2025-08-05/`
- For any date in the week of August 12-18: create `week-2025-08-12/`
- For any date in the week of August 19-25: create `week-2025-08-19/`

## File Templates

### month_plan.md
- Monthly theme and focus areas
- Key objectives and deliverables
- Important dates and deadlines
- Resource allocation

### week_plan.md
- Weekly priorities (3-5 maximum)
- Time blocks and scheduling
- Key meetings and commitments
- Success metrics

### day_DD.md
- Daily priorities (1-3 maximum)
- Time-blocked schedule
- Energy and focus allocation
- End-of-day review

## AI Navigation Benefits

This structure allows AI assistants to easily:
- **Find current planning context** using simple date calculations
- **Navigate between time horizons** (day → week → month) without complex math
- **Create new folders** automatically using consistent Monday-date naming
- **Provide time-relevant recommendations** based on clear date context

## Sample Structure

The `2025/07-july/week-2025-07-28/` folder contains sample files showing the expected format and content structure.