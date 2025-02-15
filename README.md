### Redux Heroes Management App

This project demonstrates the implementation of a Redux-based state management system for a Heroes Management application. The app allows users to fetch, filter, add, and delete heroes, showcasing key Redux concepts such as slices, async thunks, entity adapters, and selectors. The project also integrates React for the UI and Redux Toolkit for efficient state management.<br>

## Features
Fetch Heroes: Load heroes from a mock API using createAsyncThunk.<br>
<br>
Filter Heroes: Filter heroes by their element (fire, water, wind, earth) using Redux selectors.<br>
<br>
Add Heroes: Add new heroes to the list with a form, dispatching actions to update the Redux store.<br>
<br>
Delete Heroes: Remove heroes from the list, updating the store and the UI dynamically.<br>
<br>
Loading States: Handle loading and error states during API requests.<br>
<br>
Optimized State Management: Use createEntityAdapter for normalized state management and efficient updates.<br>

## Technologies Used

1) Redux Toolkit: For state management, including slices, async thunks, and entity adapters.

2) React: For building the user interface.

3) React-Redux: For connecting React components to the Redux store.

4) React Transition Group: For smooth animations when adding/removing heroes.

5) Fetch API: For making HTTP requests to the mock backend.

6) UUID: For generating unique IDs for new heroes.

## Key Redux Concepts Demonstrated
1. Slices
heroesSlice: Manages the state of heroes, including fetching, adding, and deleting heroes.

filtersSlice: Manages the state of filters and the active filter selection.

2. Async Thunks
fetchHeroes: Fetches heroes from the API.

fetchFilters: Fetches available filters from the API.

3. Entity Adapters
createEntityAdapter: Used in both heroesSlice and filtersSlice to normalize and manage collections of entities (heroes and filters).

4. Selectors
filteredHeroesSelector: Combines the list of heroes and the active filter to return filtered heroes.

selectAll: Provided by createEntityAdapter to select all entities from the state.

5. Action Dispatching
Actions like heroCreated, heroDeleted, and filtersChanged are dispatched to update the state.
