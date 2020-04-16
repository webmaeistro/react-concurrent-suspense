# react-datafetch-suspense-used

testing suspense experimental-react

React 16.6 added a <Suspense> component that lets you “wait” for some code to load and declaratively specify a loading state (like a spinner) while we’re waiting:

```
const ProfilePage = React.lazy(() => import('./ProfilePage')); // Lazy-loaded

// Show a spinner while the profile is loading
<Suspense fallback={<Spinner />}>
  <ProfilePage />
</Suspense>
```
Suspense for Data Fetching is a new feature that lets you also use <Suspense> to declaratively “wait” for anything else, including data. This page focuses on the data fetching use case, but it can also wait for images, scripts, or other asynchronous work.
