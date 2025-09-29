# Native Javascript

1. Copy the html code by <strong>selecting</strong> the non profit that you want to promote from our [Widget Copy Page](https://givelink.app/charities/widget-gen)

   ![Copy Code](/assets/widget-gen.png)

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
