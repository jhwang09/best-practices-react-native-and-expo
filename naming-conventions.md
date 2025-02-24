## Component Naming: PascalCase

- The **component itself**, as defined in your code, should be named using **PascalCase**. This means the first letter of each word is capitalized (e.g., `UserProfile`, `ChatScreen`).
- This is a standard convention in React and React Native because:
  - It distinguishes components from regular JavaScript functions or variables.
  - React uses PascalCase to identify components in JSX. For example, `<UserProfile />` clearly indicates that `UserProfile` is a component.

Here’s an example of a component definition:

```jsx
function UserProfile() {
  return <View>...</View>;
}
```

## File Naming: kebab-case

- The **file name** containing the component should use **kebab-case**, where words are separated by hyphens and all letters are lowercase (e.g., `user-profile.js`).
- This is a common practice in JavaScript projects because:
  - It avoids issues with case sensitivity across different operating systems (like Linux, macOS, or Windows).
  - It makes file names more readable and consistent in the file system.
- While camelCase (e.g., `userProfile.js`) is sometimes used, kebab-case is more widely preferred for files.

## Putting It Together

Here’s how it looks in practice:

- **Directory**: `user-profile/` (kebab-case for consistency with file naming)
- **File**: `user-profile.js` (kebab-case)
- **Component inside the file**: `UserProfile` (PascalCase)

Example file (`user-profile.js`):

```jsx
function UserProfile() {
  return <View>...</View>;
}

export default UserProfile;
```

Then, in your app, you’d use it like this:

```jsx
import UserProfile from "./user-profile";

function App() {
  return <UserProfile />;
}
```

## Why This Matters

- **Clarity**: PascalCase for components makes it obvious they’re React components, while kebab-case for files keeps the file system organized.
- **Consistency**: Following these conventions makes your codebase easier to navigate, especially for other developers or collaborators.
