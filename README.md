# README

# Steps to reproduce

1. `npm i`
2. open `node_modules/gatsby-plugin-netlify-cms/gatsby-browser.js` and add the following at line 11 inside the callback:

```javascript
console.log("Gatsby-plugin-netlify-cms: onInitialClientRender Called");
```

3. gatsby develop
4. Navigate to `https://localhost:8000/admin/

# Result

The message is never output to the console, so the callbacks are never added.

# Expected

The message is output to the console and the callbacks are added.
