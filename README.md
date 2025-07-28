
# 🖥️ newtab-terminal

A minimalist custom new tab page styled like a Linux terminal, using the beautiful 🧋 **Catppuccin Mocha** color palette.

Includes a fake prompt with a blinking cursor, keyboard focus, Google search, and easy bookmark organization — all with zero dependencies.

<img width="1364" height="463" alt="image" src="https://github.com/user-attachments/assets/c4ffa933-b036-4df1-bf55-3451193b3df7" />


---

## ✨ Features

- 🎨 Catppuccin Mocha color scheme
- 🧭 Custom bookmark grid, categorized by section
- 🔍 Fake shell prompt with Google search
- ⌨️ Typing autofocus + animated terminal-style cursor
- ⚡ Instant load, no dependencies or frameworks
- 🧠 Fully editable with just a text editor

---

## 🚀 Setup Instructions

1. **Download** or clone this repo:
   ```bash
   git clone https://github.com/TRristan/newtab-terminal.git

Open the file newtab.html in your browser to test.

Set it as your new tab page:

Chrome: Install New Tab Redirect and point it to your local newtab.html

Firefox: Use Custom New Tab or modify user preferences via about:config

🛠️ Customization Guide
🔗 Editing bookmarks
Bookmarks are inside the <nav> tag in newtab.html. Each column is an unordered list (<ul>) with a header and a list of links:

```html

<ul>
  <li>general</li>
  <li><a href="https://example.com">my link</a></li>
  <li><a href="https://another.com">another one</a></li>
</ul>
```
Each section auto-gets a different Catppuccin accent (pink, peach, yellow, green, teal...).

You can add, remove, or rename categories freely.

🔍 Search engine customization
The fake shell prompt uses Google by default. You can change the search provider in the <script> tag at the bottom:
```js


window.location.href = `https://www.google.com/search?q=${encodeURIComponent(query)}`;
```
To switch to another engine:

🦆DuckDuckGo:
```js

`https://duckduckgo.com/?q=${encodeURIComponent(query)}`
```
