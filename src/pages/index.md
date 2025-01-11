---
layout: ../layouts/Layout.astro
---

# Ez Dialogs

Ez Dialogs is a lightweight library to make using the &lt;dialog&gt; element intuitive and easy.

1. Install the package:

```bash
npm install ez-dialogs
```

2. Import the CSS & EzDialog. You can import the CSS elsewhere if needed.

```js
import "ez-dialogs/style.css";
import EzDialog from "ez-dialogs";
```

3. Create a new instance of EzDialog:

```js
const ezDialogMain = new EzDialog(
  document.querySelector("[ez-dialog]"),
  "main",
);
```

4. Add the required HTML. The content used is provided only as an example, use your own content.

```html
<dialog class="ez-dialog">
  <button ez-dialog-close="main" class="ez-dialog-close">X</button>
  <div ez-dialog-content="main" class="ez-dialog-content">
    <h1>Dialog Example</h1>
    <p>This is an example dialog.</p>
  </div>
</dialog>
```

5. Add the correct attribute anywhere you want the dialog to be openable.

```html
<button ez-dialog-trigger="main">Open</button>
```