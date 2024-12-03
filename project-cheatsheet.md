# Quick Reference for Web Development

## Variables

- Define reusable variables for consistency and maintainability.

```CSS
:root {
  --orange: #f42;
  --light-grey: rgb(231, 221, 221);
  --yellow: #fd3;
  --black: #131313;
  --light-white: hsla(0, 0%, 100%, 0.6);
  --white: #fff;
  --grey-white: #aaa;
  --white-opaque: #fff9;
}

```

## CSS Reset

```CSS
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
```

##  Page Layout and Structure

- The project employs CSS Flexbox for layout and alignment and avoids complex frameworks.

```CSS
body {
  display: flex;
  flex-direction: column;
  overflow-x: hidden;
  height: 100%;
}

.header {
  position: fixed;
  width: 100%;
  background-color: #fff;
  z-
  index: 1;
}
.footer {
  display: block;
  background-color: #333;
  color: #fff;
  padding: 10px;
}
```

## Media Queries and Responsiveness

- Adaptability to different screen sizes is achieved using media queries.

```CSS
@media (max-width: 768px) {
  .header-images {
    grid-template-columns: 1fr; /* Stack on smaller screens */
  }
  .mobile {
    display: block;
  }
}

@media (min-width: 1024px) {
  .header-images {
    grid-template-columns: repeat(3, 1fr); /* Return to 3 columns */
  }
}

```
