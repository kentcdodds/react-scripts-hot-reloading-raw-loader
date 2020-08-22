# v4 regression on hot reloading of raw-loader content

```javascript
// eslint-disable-next-line import/no-webpack-loader-syntax
import html from '!raw-loader!./example.html'
document.body.innerHTML = html
```

Changing `example.html` triggers a refresh in `react-scripts@v3`, but not in
`react-scripts@v4`.
