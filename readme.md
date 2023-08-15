# Using `prefers-color-scheme` media query to change theme

Giving users the ability to toggle a theme themselves is great, but there’s another option for setting a theme that you may have come across on certain sites or applications: using the user’s theme setting from their operating system or user agent (like a browser). This can be accomplished with the prefers-color-scheme media query, which simply checks whether a user has selected a theme preference on their OS/user agent. In the live application, try changing the theme settings on your OS/user agent to see how the example updates in real time!

This [example](https://www.theodinproject.com/lessons/node-path-intermediate-html-and-css-custom-properties#creating-themes-with-custom-properties:~:text=our%20root%20element.-,Media%20queries,-Giving%20users%20the) is a part of The Odin Project curriculum.

## Features

- Automatically matches your system theme

## Snippets

```css
:root {
  --border-btn: 1px solid rgb(36, 36, 36);
  --color-base-bg: rgb(240, 240, 240);
  --color-base-text: rgb(18, 18, 18);
  --color-btn-bg: rgb(220, 220, 220);
  --theme-name: 'light';
}

@media (prefers-color-scheme: dark) {
  :root {
    --border-btn: 1px solid rgb(220, 220, 220);
    --color-base-bg: rgb(18, 18, 18);
    --color-base-text: rgb(240, 240, 240);
    --color-btn-bg: rgb(36, 36, 36);
    --theme-name: 'dark';
  }
}
```
