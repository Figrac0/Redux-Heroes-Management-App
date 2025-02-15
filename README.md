# Redux Heroes Management App (RTK Query Branch)

This branch demonstrates the integration of Redux Toolkit Query (RTK Query) into the Heroes Management application. RTK Query simplifies data fetching and caching, replacing manual HTTP requests and state management with a more efficient and declarative approach.

## Key Changes in This Branch

1. RTK Query Integration
Replaced manual fetch calls with RTK Query's createApi for data fetching and caching.

Implemented endpoints for:

Fetching heroes (getHeroes).

Creating a new hero (createHero).

Deleting a hero (deleteHero).

2. Tag-based Cache Invalidation
Used providesTags and invalidatesTags to automatically manage cache updates:

Fetching heroes provides the 'Heroes' tag.

Creating or deleting a hero invalidates the 'Heroes' tag, triggering a refetch of the heroes list.

3. Simplified Code
Removed custom hooks like useHttp and manual Redux thunks.

Reduced boilerplate code by leveraging RTK Query's built-in features.

## Technologies Used
Redux Toolkit Query (RTK Query): For data fetching, caching, and cache invalidation.

Redux Toolkit: For state management and API slice creation.

React: For building the user interface.

React-Redux: For connecting React components to the Redux store.
