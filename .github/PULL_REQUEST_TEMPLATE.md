Add persistent database storage using SQLite

## Changes
- Replaced in-memory activities dictionary with SQLite database for persistence
- Created `activities` and `participants` tables
- Database initializes with existing data on first run
- Updated all API endpoints to interact with the database
- Added validation to prevent signing up for full activities
- Data now survives server restarts

## Benefits
- **Persistence**: Activities and signups are saved permanently
- **Scalability**: Can handle more data without memory constraints
- **Reliability**: No data loss on crashes or restarts
- **Foundation**: Enables future features like user management and advanced queries

## Testing
- App starts without errors
- Database file created successfully
- Existing functionality preserved
- New signup validation added

Closes #9