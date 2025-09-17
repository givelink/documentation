# Native Javascript

1. Copy the html code that it is provided in the [Charity Interface](https://ci.givelink.app).

![Copy Code](/assets/ci-1.png)
![Copy Code](/assets/ci-2.png)

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
