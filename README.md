# KeyUX

JS library to improve keyboard UI of web apps. It was designed not only
for **a11y** but also to create **professions tools** where users prefer
using keyboard.

* Add **hotkeys** support by `aria-keyshortcuts`.
* Show button’s `:active` state when user press hotkey.
* Enable **arrows navigation** in `role="menu"` lists.
* Jump to next section according to `aria-controls` and back by <kbd>Esc</kbd>.
* Show/hide submenus of `role="menu"`.
* Allows users to **override hotkeys**.
* **1 KB** (minified and brotlied). No dependencies.

```jsx
export const Button = ({ hokey, children }) => {
  return <button aria-keyshortcuts={hotkey}>
    {children}
    {likelyWithKeyboard(window) && <kbd>{getHotKeyHint(window, hotkey)}</kbd>}
  </button>
}
```

---

<img src="https://cdn.evilmartians.com/badges/logo-no-label.svg" alt="" width="22" height="16" />  Made in <b><a href="https://evilmartians.com/devtools?utm_source=keyux&utm_campaign=devtools-button&utm_medium=github">Evil Martians</a></b>, product consulting for <b>developer tools</b>.

---

## Install

```sh
npm install keyux
```
