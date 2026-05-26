# Native Javascript

## Option A – Button

Follow [this](https://youtu.be/RYr3XJ6BTF4) step by step video, or read the steps below:

1. Copy the html code by <strong>selecting</strong> the non profit that you want to promote from our [Widget Copy Page](https://givelink.app/charities/widget-gen)

   ![Copy Code](/assets/widget-assets-english.png)

2. Paste it into your website where you want the button to appear

3. Add a button or link that has `onClick={() => window.Givelink?.open?.()}` or has the class `givelink-button`.

eg.

```html
<button class="givelink-button">Donate</button>
```

or

```html
<button onclick="window.Givelink?.open?.()">Donate</button>
```

---

## Option B – Inline Widget

The widget is displayed directly on the page — no button click needed. Visitors see it immediately when they arrive.

1. In the [Widget Generator](https://givelink.app/charities/widget-gen), select the **Inline** tab and copy the embed code
2. Paste it directly into your HTML where you want the widget to appear:
   ```html
   <!-- Paste your Givelink inline embed code here -->
   ```
3. Deploy your changes

> 💡 **Tip:** The inline embed code (Option B) is different from the popup script (Option A). Make sure to select the correct tab in the Widget Generator.

---

## Typescript

In case of typescript, you may need to extend the `window` type if you want to use `window.Givelink.open()`.

To do so, you need to add the following code to a `.d.ts` file in your project:

```typescript
interface Window {
  Givelink?: {
    open: () => void;
  };
}
```
