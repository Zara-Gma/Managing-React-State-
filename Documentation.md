- If you forget what properties are available on event, set a debugger and inspect the event

## When does React render?

- State change
  > Can skip render via: shouldComponentUpdateReact.Memo
- Prop change
  > Can skip render via: shouldComponentUpdateReact.Memo PureComponent
- Parent renders
  > Can skip render via: shouldComponentUpdateReact.Memo PureComponent
- Context change
  > React won't re-render when a plain variable changes
  > When state changes, the component renders, which causes derived state to be recalculated
  > So derived state can't get out of sync, it's recalculated on each render

## Four ways to handle API Calls

- Inline
  > Call fetch / Axios / etc in your component (Not recommended)
- Centralized functions
  > Call separate function
- Custom hook
  > Create and call your own custom hook
- Library
  > Call library (react-query, swr, etc)
