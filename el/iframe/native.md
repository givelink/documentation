# Native Javascript

Ακολουθήστε [αυτό](https://youtu.be/RYr3XJ6BTF4) το βίντεο βήμα προς βήμα, ή διαβάστε τα παρακάτω βήματα:

1. Αντιγράψτε τον κώδικα HTML <strong>επιλέγοντας</strong> την ΜΚΟ που θέλετε να προωθήσετε από τη [Σελίδα Αντιγραφής Widget](https://givelink.app/charities/widget-gen)

   ![Αντιγραφή Κωδικού](/assets/widget-assets-greek.png)

2. Επικολλήστε τον στον ιστότοπό σας εκεί όπου θέλετε να εμφανίζεται το κουμπί

3. Προσθέστε ένα κουμπί ή σύνδεσμο που έχει `onClick={() => window.Givelink?.open?.()}` ή έχει την κλάση `givelink-button`.

π.χ.

```html
<button class="givelink-button">Donate</button>
```

ή

```html
<button onclick="window.Givelink?.open?.()">Donate</button>
```

## Typescript

Σε περίπτωση typescript, ενδέχεται να χρειαστεί να επεκτείνετε τον τύπο `window` εάν θέλετε να χρησιμοποιήσετε το `window.Givelink.open()`.

Για να το κάνετε αυτό, πρέπει να προσθέσετε τον παρακάτω κώδικα σε ένα αρχείο `.d.ts` στο έργο σας:

```typescript
interface Window {
  Givelink?: {
    open: () => void;
  };
}
```
