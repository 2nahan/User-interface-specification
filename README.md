# User Management Screen UI Specification

## Requirements
1. **View Users**: Display a list of all users with ID, username, email, and enabled status.
2. **Add User**: Provide a form to add a new user.
3. **Edit User**: Allow editing of existing user details.
4. **Hide Disabled Users**: Option to hide/show disabled users.
5. **Save User**: Save new or edited user details.
6. **User Roles Management**: Manage user roles (Guest, Admin, SuperAdmin).

## UI Components

### User List Table
- **Columns**:
  - ID
  - User Name
  - Email
  - Enabled
- **Rows**: Each row represents a user.
- **Sorting**: Sortable columns.
- **Filtering**: Filter by enabled status.

### New User Button
- **Button**: Opens the form to add a new user.(Top-left)

### Hide Disabled Users Checkbox
- **Checkbox**: Toggles visibility of disabled users. (Next to the New User Button)

### User Form (New/Edit User)
- **Fields**:
  - Username (Text)
  - Display Name (Text)
  - Phone (Text)
  - Email (Email)
  - User Roles (Dropdown)
  - Enabled (Checkbox)
- **Save User Button**: Submits form to save user details. (Right side)

## At the Beginning
- Display User List Table with all users.
- New User Button visible.
- Hide Disabled Users Checkbox unchecked.
- User Form fields empty, Save User Button disabled.

## Behavior

### User List Table
- **Default View**: Display all users sorted by ID.
- **Sorting**: Click column headers to sort.
- **Filtering**: Filter by enabled status.

### New User Button
- **Click**: Opens User Form for adding a user, clearing any existing values.

### Hide Disabled Users Checkbox
- **Checked**: Hides disabled users.
- **Unchecked**: Shows all users.

### User Form (New/Edit User)
- **Save Button**: Enabled when all required fields are filled.
  - **Save**: Adds or updates user in the User List Table.
  - **Validation**: Ensures valid email and non-empty required fields.
- **Edit User**: Pre-fills form with selected user’s details.

## Error Handling
- **Form Validation**: Shows errors for invalid inputs or missing fields.
- **Save Errors**: Displays notification if saving fails.

## Success Messages
- **Add/Edit**: Shows message on successful addition or update.
