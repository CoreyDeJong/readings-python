## React Router
 - `npm install react-router-dom`
 - the basic router has 3 “pages”: a home page, an about page, and a users page. As you click around on the different <Link>s, the router renders the matching <Route>.
 - nested routing: The route /topics loads the Topics component, which renders any further <Route>'s conditionally on the paths :id value.

## React - Styling
- “CSS-in-JS” refers to a pattern where CSS is composed using JavaScript instead of defined in external files
```
render() {
  return <span className="menu navigation-menu">Menu</span>
}
```

## NextJS
- An intuitive page-based routing system (with support for dynamic routes)
- Pre-rendering, both static generation (SSG) and server-side rendering (SSR) are supported on a per-page basis
- Automatic code splitting for faster page loads
- Client-side routing with optimized prefetching
- Built-in CSS and Sass support, and support for any CSS-in-JS library
- Development environment which supports Hot Module Replacement
- API routes to build API endpoints with Serverless Functions
- Fully extendable