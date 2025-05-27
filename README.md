# 📚 React Cheatsheets

### Comprehensive React.js cheatsheets: your quick reference guide to mastering React's core concepts and techniques.

| Cheatsheet Name                    | Description                                                                                                                                                                                               | Links                                                                                                  |
| ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| devhints React cheat sheet          | React is a JavaScript library for building user interfaces. This guide targets React v15 to v16.                                                                                                          | [devhints](https://devhints.io/react)                                                                  |
| SheCodes React Cheat sheet          | Comprehensive React cheat sheet for beginners.                                                                                                                                                             | [shecodes](http://cheatsheets.shecodes.io/cheatsheets/react/events)                                    |
| React Typescript Cheat sheet        | React has documentation for how to start a new React project with some of the most popular frameworks. Here's how to start them with TypeScript.                                                          | [react typescript](https://react-typescript-cheatsheet.netlify.app/docs/basic/setup)                   |
| Louis' React Cheat sheet           | You can find cheat sheets and general resources, containing examples, of different technologies. These technologies include programming languages, frameworks, and libraries I am personally interested in. | [codehints](https://codehints.io/category/react)                                                       |
| logrocket's React-Hooks cheat sheet | This React Hooks cheat sheet includes a lot of code snippets and assumes some Hooks fluency.                                                                                                              | [logrocket react hooks](https://blog.logrocket.com/react-hooks-cheat-sheet-solutions-common-problems/) |
| React-Hooks cheat sheet             | A cheat sheet with live editable examples and one-stop reference for hooks.                                                                                                                                | [react hooks](https://react-hooks-cheatsheet.com/)                                                     |
| Freecodecamp React cheat sheet      | a super helpful cheat sheet to give you a complete overview of all of the React concepts you need to know.                                                                                                 | [freecodecamp react cheat sheet](https://www.freecodecamp.org/news/the-react-cheatsheet/)               |
| CodeCademy React cheat sheet | Codecademy has hundreds of free and easy-to-use cheat sheets that cover dozens of coding languages and are created by our world-class curriculum developers. | [CodeCademy react cheatsheet](https://www.codecademy.com/learn/react-101/modules/react-101-jsx-u/cheatsheet) |


### React Video tutorials & Articles

| Resource Name                    | Description                                                                                                                                                                                               | Links                                                                                                  |
| ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| React Resources | React articles & tutorials | [React Resources](https://www.freecodecamp.org/news/the-react-cheatsheet/)               |
| React Official website | React.dev serves as the primary source for official React documentation. It provides comprehensive guides, tutorials, and reference materials for developers who want to learn and work with React. | [React.dev](https://react.dev/learn#) |
| React Introduction by Kent C. Dodds | A free, concise video course covering essential React concepts like JSX, conditional rendering, forms, styling, lists, HTTP requests, and app deployment. | [ egghead react Course by Kent ](https://egghead.io/lessons/react-a-beginners-guide-to-react-introduction) |



# 🎯 React interview prep. topics

### Introduction to React
- Component-Based
- Declarative UI
- Virtual DOM
- JSX
- SPA (Single Page Application)
- React Server Components - Render components on the server to improve performance and reduce bundle size.
- Allows React to interrupt rendering to keep the app responsive.
- Suspense for Data Fetching - Show fallback UI while waiting for async data to load.
- Automatic Batching - Groups multiple state updates into one render for better performance.

### Diffrent ways of React setup
Each of these methods installs React, but differs in how it bundles and runs the app:
1. Next.js - Includes routing, SSR support
```
npx create-next-app@latest my-app
cd my-app
npm run dev
```
2. Vite + React - Fastest build tool, modern, lightweight
```
npm create vite@latest my-app --template react
cd my-app
npm install
npm run dev
```
3. CRA ( Create React App ) - Slower build, works out of the box
```
npx create-react-app my-app
cd my-app
npm start
```
4. Manual - Full control over configuration ( Best if you want to learn internals )
```
mkdir my-app
cd my-app
npm init -y

npm install react react-dom
npm install -D webpack webpack-cli webpack-dev-server babel-loader @babel/core @babel/preset-env @babel/preset-react html-webpack-plugin
```


### Basics in React
- JSX Syntax - 	HTML-like syntax used in React to write UI code inside JavaScript.
- Functional - Components written as functions, often using React Hooks ex. useState(), useEffect() etc.
- Components - Reusable UI parts that return JSX.
- Props - Data passed to components to customize their content or behavior.

### Hooks
| Hook |	Purpose |
|------|------------|
|useState |	Manage local state inside functional components.|
|useEffect |	Run side effects like data fetching or subscriptions.|
|useRef |	Reference DOM elements or keep values across renders (no re-renders).|
|useContext |	Share values globally without prop drilling.|
|useReducer |	Handle complex state logic using actions (like Redux lite).|
|useMemo |	Cache expensive calculations to improve performance.|
|useCallback |	Cache function definitions to prevent unnecessary re-renders.|
|useLayoutEffect |	Like useEffect, but runs before the browser paints the screen.|
|useImperativeHandle |	Customize what ref exposes to parent components.|
|useDebugValue |	Show custom hook values in React DevTools for debugging.|
|useId |	Generate stable unique IDs (useful for accessibility).|

### Component Communication
| Term | Meaning |
|------|------------|
|Props Drilling | Passing data through many components. |
|Context API | 	Share data without passing props everywhere. |
|State Lifting | Move shared data to the parent component. |
|Event Handlers | Functions passed as props to handle events in child components (e.g., onClick). |

### Rendering Techniques
- Conditional Rendering - Show/hide UI based on conditions (e.g., if, ? :, &&).
- Lists with.map() - Render multiple elements by looping through an array.
- Keys in Lists - Unique identifiers used in .map() to help React track items efficiently.

### Forms
- Controlled Components - Controlled components keep the input value in React’s state, so React always knows what the user has typed ( text/value entered by the user in the input field), controls what’s displayed, and updates state on input changes.
- Uncontrolled Components - Inputs that keep their own state inside the browser (not in React), and you get their values using ```refs``` instead of React state.
- Input Handling
- Form Submission 
- Basic Validation

### React Router (v6)
| Feature |	Description |
|----------------|-----------------------------------------|
| BrowserRouter |	Wraps your app enabling routing using browser history API.|
| Routes & Route |	Define URL paths and the components to render.|
| Link & NavLink |	Navigate without page reload; NavLink adds active styles.|
| Dynamic Routing |	Routes with URL parameters (e.g., /user/:id).|
| 404 Page |	Catch-all route for unmatched URLs (shows Not Found page).|
| Outlet |	Placeholder to render nested child routes inside parent routes.|
| Navigate |	Programmatic navigation/redirect in your app.|
| useParams |	Hook to access dynamic route parameters inside components.|

### APIs & Fetching Data
| Topic |	Description |
|------------|----------------------------------|
| fetch & axios |	Methods to make HTTP requests; fetch is native, axios is a popular library with extra features. |
| REST vs GraphQL |	REST is a traditional API style with fixed endpoints; GraphQL lets clients ask for exactly the data they need. ex. <table><thead><tr><th>REST</th></tr></thead><tbody><tr><td><code>fetch('https://api.example.com/users/1').then(res => res.json()).then(data => console.log(data)).catch(err => console.error(err));</code></td></tr></tbody></table><table><thead><tr><th>GraphQL</th></tr></thead><tbody><tr><td><code>fetch('https://api.example.com/graphql', { method: 'POST', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify({ query: `{ user(id: 1) { id name email } }` }) }).then(res => res.json()).then(data => console.log(data.data.user)).catch(err => console.error(err));</code></td></tr></tbody></table> |
| Loading States |	Indicate to users when data is being fetched (e.g., spinners or messages). |
| Error Handling |	Manage errors from API calls gracefully (show error messages, retry logic). |
| Caching |	Store fetched data to improve performance and reduce unnecessary requests. |
| Async/Await |	Modern syntax to handle asynchronous API calls clearly and cleanly. |

### Optimization & Best Practices
| Concept |	Description |
|------------|----------------------------------|
| Code Splitting | Load components only when needed using React.lazy() & Suspense.
| Memoization |	Use React.memo ( Stops re-rendering a component if its props didn’t change ), useMemo ( Cache a value ), useCallback (	Cache a function ) to avoid unnecessary recalculations or re-renders. |
| Avoid Re-renders | Prevent extra renders by lifting state smartly, memoizing props/functions. |
| Folder Structure | Keep folders modular and well-organized (e.g., components/, hooks/, pages/). |
| Lazy Loading | Defer loading of non-critical components/pages to improve initial performance. |
| Use Keys Properly | Use unique, stable keys in list items to help React with efficient DOM updates. |
| State Management | Use context, Redux, or Zustand wisely to prevent unnecessary global re-renders. |
| Component Size | Break down large components into smaller, focused units for readability and reuse. |
| Image Optimization | Use correct formats, compression, and lazy loading for better performance. |
| Avoid Inline Functions | Define functions outside of render to prevent re-creating them on every render. |
| Throttle/Debounce | Use in event-heavy areas (e.g., search inputs, scroll events) to improve performance. |

### TypeScript with React
| Topic | Description |
|-----------------|-------------------------|
| Typed Props & State |	Define types for props and state to catch errors early.|
| Interfaces |	Create reusable type shapes for props or objects. |
| ```useState<Type>``` |	Specify the type your state holds for type safety. |
| Optional Props |	Use ? to mark props as optional. |
| Type Aliases |	Another way to define types, often for unions or primitives. |
| Generics |	Make components or hooks flexible with generic types. |
| Type Inference |	TypeScript often guesses types, so you don’t always need to specify. |
| React.FC vs Function Components |	React.FC includes implicit children types, but some | 
| prefer | plain functions for flexibility. |

### Lifecycle Methods (Class Components)
| Method | Description |
|----------------|-----------------|
| constructor() |	Initializes state and binds methods before mounting. |
| render() | Returns JSX to display UI, runs on every update. |
| componentDidMount()	Runs once after the component is added to the DOM (good for fetching data). |
| componentDidUpdate() |	Runs after updates (props or state change), useful for side effects. |
| componentWillUnmount() | Runs before component is removed from the DOM (cleanup like timers). |

### Higher Order Components (HOCs)
| Topic |	Simple Explanation |
|----------------|-----------------|
| withAuth(Component) | Wraps a component to add authentication logic. |
| withLogger(Component) | Wraps a component to log props or actions for debugging. |
| Reusability | HOCs help reuse common logic across many components. |
| Code Wrapping | HOCs wrap a component to enhance or modify its behavior. |
| Naming Convention | Always name HOCs starting with with (e.g., withTheme). |

```
// Example of HOC
import React from 'react';

// HOC that logs props
function withLogger(WrappedComponent) {
  return function LoggerComponent(props) {
    console.log('Props:', props);
    return <WrappedComponent {...props} />;
  };
}

// Usage example:
function Hello(props) {
  return <h1>Hello, {props.name}!</h1>;
}

const HelloWithLogger = withLogger(Hello);

// In your app render:
// <HelloWithLogger name="Alice" />


// withLogger takes any component and returns a new one that logs props before rendering it.
// This way, you add logging logic without changing the original component.
```

### Advanced Features
- Fragments (<> </>) - Group multiple elements without adding extra DOM nodes.
- StrictMode - Helps find potential problems by running extra checks in development.
- Portals - Render components outside the main DOM tree (e.g., modals).
- Error Boundaries - 	Catch errors in components to prevent app crashes and show fallback UI.
- Lazy Loading - 	Load components only when needed using ```React.lazy()``` and ```Suspense```.

### Testing
- Jest - Popular testing framework for running unit and integration tests.
- React Testing Library - Focuses on testing UI by simulating user behavior, encouraging good testing practices.
- Snapshot Testing - Saves rendered UI output to detect unexpected changes over time.
- Hook Testing - Testing custom React hooks independently, often using @testing-library/react-hooks.
- Mocking - Simulate API calls or modules to isolate tests.
- End-to-End (E2E) Testing - Tools like Cypress or Playwright test full user flows in the browser.

### Custom Hooks
1. useLocalStorage() - Stores and retrieves a value from localStorage.
```
function useLocalStorage(key, initialValue) {
  const [storedValue, setStoredValue] = useState(() => {
    try {
      const item = window.localStorage.getItem(key);
      return item ? JSON.parse(item) : initialValue;
    } catch {
      return initialValue;
    }
  });

  const setValue = (value) => {
    try {
      setStoredValue(value);
      window.localStorage.setItem(key, JSON.stringify(value));
    } catch {}
  };

  return [storedValue, setValue];
}
```

2. useWindowSize() - Tracks window width and height.
```
function useWindowSize() {
  const [size, setSize] = useState({ width: window.innerWidth, height: window.innerHeight });

  useEffect(() => {
    function handleResize() {
      setSize({ width: window.innerWidth, height: window.innerHeight });
    }
    window.addEventListener('resize', handleResize);
    return () => window.removeEventListener('resize', handleResize);
  }, []);

  return size;
}
```
3. useDarkMode() - Detects and toggles dark mode.
```
function useDarkMode() {
  const [isDark, setIsDark] = useState(() => window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches);

  useEffect(() => {
    const listener = e => setIsDark(e.matches);
    window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', listener);
    return () => window.matchMedia('(prefers-color-scheme: dark)').removeEventListener('change', listener);
  }, []);

  const toggleDarkMode = () => setIsDark(prev => !prev);

  return [isDark, toggleDarkMode];
}
```
4. useDebounce() - Delays a value update until after a wait time.
```
import { useState, useEffect } from 'react';

function useDebounce(value, delay) {
  const [debouncedValue, setDebouncedValue] = useState(value);

  useEffect(() => {
    const handler = setTimeout(() => setDebouncedValue(value), delay);
    return () => clearTimeout(handler);
  }, [value, delay]);

  return debouncedValue;
}
```
5. useThrottle() - Limits how often a function can run.
```
import { useRef, useEffect } from 'react';

function useThrottle(callback, delay) {
  const lastCall = useRef(0);

  return (...args) => {
    const now = Date.now();
    if (now - lastCall.current >= delay) {
      lastCall.current = now;
      callback(...args);
    }
  };
}
```
6. useFetch() - Fetch data with loading & error states
```
import { useState, useEffect, useCallback } from 'react';

function useFetch(url, options) {
  const [data, setData] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  const fetchData = useCallback(async () => {
    setLoading(true);
    setError(null);
    try {
      const response = await fetch(url, options);
      if (!response.ok) throw new Error('Network response was not ok');
      const json = await response.json();
      setData(json);
    } catch (err) {
      setError(err.message || 'Something went wrong');
    } finally {
      setLoading(false);
    }
  }, [url, options]);

  useEffect(() => {
    fetchData();
  }, [fetchData]);

  return { data, loading, error, refetch: fetchData };
}
```

7. usePrevious() — Track previous value
```
import { useRef, useEffect } from 'react';

function usePrevious(value) {
  const ref = useRef();
  useEffect(() => {
    ref.current = value;
  }, [value]);
  return ref.current;
}
```

8. useClickOutside — Detect clicks outside a ref element
```
import { useEffect } from 'react';

function useClickOutside(ref, handler) {
  useEffect(() => {
    function listener(event) {
      if (!ref.current || ref.current.contains(event.target)) return;
      handler(event);
    }
    document.addEventListener('mousedown', listener);
    document.addEventListener('touchstart', listener);
    return () => {
      document.removeEventListener('mousedown', listener);
      document.removeEventListener('touchstart', listener);
    };
  }, [ref, handler]);
}
```

9. useEventListener — Add and clean up event listeners
```
import { useEffect, useRef } from 'react';

function useEventListener(eventName, handler, element = window) {
  const savedHandler = useRef();

  useEffect(() => {
    savedHandler.current = handler;
  }, [handler]);

  useEffect(() => {
    if (!(element && element.addEventListener)) return;
    const eventListener = (event) => savedHandler.current(event);
    element.addEventListener(eventName, eventListener);
    return () => element.removeEventListener(eventName, eventListener);
  }, [eventName, element]);
}
```
```
// How to use useEventListener
function WindowSize() {
  const [size, setSize] = React.useState({
    width: window.innerWidth,
    height: window.innerHeight,
  });

  useEventListener('resize', () => {
    setSize({ width: window.innerWidth, height: window.innerHeight });
  });

  return (
    <div>
      Window size: {size.width} x {size.height}
    </div>
  );
}
```

10. useOnScreen — Detect if element is visible in viewport
```
import { useState, useEffect, useRef } from 'react';

function useOnScreen(options) {
  const ref = useRef();
  const [isIntersecting, setIntersecting] = useState(false);

  useEffect(() => {
    const observer = new IntersectionObserver(
      ([entry]) => setIntersecting(entry.isIntersecting),
      options
    );
    if (ref.current) observer.observe(ref.current);
    return () => {
      if (ref.current) observer.unobserve(ref.current);
    };
  }, [ref, options]);

  return [ref, isIntersecting];
}
```

11. useToggle — Toggle boolean state easily
```
import { useState, useCallback } from 'react';

function useToggle(initialValue = false) {
  const [state, setState] = useState(initialValue);
  const toggle = useCallback(() => setState(s => !s), []);
  return [state, toggle];
}
```


### Styling
- CSS Modules - Scoped CSS for components to avoid clashes.
- Inline Styles - Styles defined directly on elements in JSX.
- Styled-Components - CSS-in-JS library for writing CSS inside JS files.
- Tailwind CSS - Utility-first CSS framework for fast styling.
- SCSS/SASS - CSS preprocessors for variables and nesting.
- CSS-in-JS - Write CSS styles directly in JavaScript (e.g., Emotion, Stitches).
- Utility-First CSS - Small reusable classes to build designs quickly (e.g., Tailwind).

### UI Libraries
- Tailwind CSS - Utility CSS framework for design flexibility.
- ShadCN/UI - Modern accessible React components built on Radix UI.
- Ant Design - Enterprise-level UI components with rich features.
- Material UI - Google’s Material Design React components.
- Chakra UI - Accessible and customizable React component library.
- Headless UI - Unstyled accessible UI components for full design control.
- Radix UI - Low-level UI primitives for building custom components.

### Common Mistakes
- Incorrect Key Props - Missing or duplicate keys in lists causing rendering issues.
- Improper State Updates - Mutating state directly instead of immutably updating.
- Infinite Loops in useEffect - Not managing dependencies properly causing endless re-renders.
- Direct DOM Manipulation - Manipulating DOM outside React can break UI consistency.
- Not Cleaning up Effects - Missing cleanup in effects can cause memory leaks or bugs.
- Overusing Context API - Using context for too many updates can hurt performance.
- Ignoring Accessibility - Skipping accessibility basics reduces usability for all users.




## ✨ Contributing

Contributing is possible via GitHub. Alternatively, you can send in content, content-drafts or content-ideas
via Mail: rcdesign28@gmail.com

## 🔗 Let's Connect

[![linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rakeshc7/)
[![twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/_Rakeshc7)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/rakesh.chotaliya7/)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](rcdesign28@gmail.com)
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://rakeshchotaliya.com/)
