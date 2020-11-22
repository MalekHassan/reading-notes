# Hooks API

**Why do we not need more .html pages in a multi-page React app?**  
With React, we can rerender separate parts of the page when we need to render them, so it appears that we are going to different pages, and the route changes, but it is just rendering different things on the same html page based on the current state.  
**If we wanted a component to show up on every page, where would we put it and why?**

- Outside the `<BrowserRouter/>`
- **Inside the `<BrowserRouter />`, outside a `<Route />`**
- Inside a `<Route />`

**What does props.children contain?**  
`props.children` contains data passsed in from the parent component that can be used in the child component.

| Term                      | Definition                                                                                                                                                                             |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Composition               | This is where a more specific component renders a more generic component configured with props.                                                                                        |
| Children/child components | Children components are given props from the parent component, and are rendered partially based on where they are in the parent component.                                             |
| Hash Routing              | A router that uses client side hash routing. It does not need any configuration in the server to handle routes, but it is mainly recommended when you need to support legacy browsers. |
| Link Routing              | With link routing, you navigate a site by being directed to different paths, and this is done in React with react-router-dom                                                           |
