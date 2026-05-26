# 🌟 Πραγματικά Παραδείγματα

Δείτε πώς μη κερδοσκοπικοί οργανισμοί χρησιμοποιούν το Givelink για να δέχονται δωρεές σε είδος στις ιστοσελίδες τους.

---

## Οργανισμοί που χρησιμοποιούν το Givelink

| Οργανισμός | Ιστοσελίδα | Τύπος Ενσωμάτωσης |
|---|---|---|
| Pilgrim Terrace | [pilgrimterrace.org/donate](https://pilgrimterrace.org/donate) | Επιλογή Α – Κουμπί |
| Swords to Plowshares | [swords-to-plowshares.org](https://www.swords-to-plowshares.org/) | Επιλογή Α – Κουμπί |
| The KSP | [theksp.org/donate-goods](https://www.theksp.org/donate-goods) | Επιλογή Α – Κουμπί |
| BOSS | [bosshelp.org/donate-goods](https://bosshelp.org/donate-goods/) | Επιλογή Β – Ενσωματωμένο Widget |
| Rock SF | [rocksf.org/donate](https://rocksf.org/donate/) | Σύνδεσμος στο Προφίλ Givelink |
| Heart to Art Collective | [hearttoartcollective.org](https://sites.google.com/view/hearttoartcollective/get-involved#h.tfcoiq7bsef0) | Σύνδεσμος στο Προφίλ Givelink |

> **Το Rock SF** και το **Heart to Art Collective** χρησιμοποιούν την πιο απλή προσέγγιση: έναν απλό υπερσύνδεσμο στην ιστοσελίδα τους που οδηγεί απευθείας στη σελίδα του προφίλ τους στο Givelink — χωρίς κώδικα ενσωμάτωσης.

---

## Επιλογή Α – Κουμπί

Ένα κουμπί τοποθετείται στη σελίδα σας. Όταν κάποιος το πατήσει, ανοίγει το widget δωρεών του Givelink σε αναδυόμενο παράθυρο. Αυτή είναι η πιο συνηθισμένη και εύκολη ενσωμάτωση.

**Οργανισμοί που χρησιμοποιούν αυτή την επιλογή:** Pilgrim Terrace · Swords to Plowshares · The KSP

### WordPress

1. Αντιγράψτε τον κώδικα ενσωμάτωσης από τη [Γεννήτρια Widget](https://givelink.app/charities/widget-gen)
2. Στον επεξεργαστή WordPress, προσθέστε ένα μπλοκ **Custom HTML** και επικολλήστε τον κώδικα
3. Προσθέστε ένα μπλοκ **Buttons** και ορίστε ως πρόσθετη κλάση CSS: `givelink-button`
4. Προσαρμόστε το κείμενο και τα χρώματα του κουμπιού ώστε να ταιριάζουν με τη σελίδα σας
5. Αποθηκεύστε και δημοσιεύστε

📖 [Πλήρης Οδηγός WordPress →](../en/iframe/wordpress.md)

---

### Squarespace

1. Αντιγράψτε τον κώδικα ενσωμάτωσης από τη [Γεννήτρια Widget](https://givelink.app/charities/widget-gen)
2. Προσθέστε ένα μπλοκ **Button** στη σελίδα σας
3. Ορίστε τον σύνδεσμο του κουμπιού ως `#givelink-button` (αφαιρέστε την επιλογή "Open in new tab")
4. Μεταβείτε στο **Custom Code → Code Injection** και επικολλήστε τον κώδικα στην ενότητα **Footer**
5. Αποθηκεύστε και δημοσιεύστε

📖 [Πλήρης Οδηγός Squarespace →](../en/iframe/squarespace.md)

---

### Wix

1. Αντιγράψτε τον κώδικα ενσωμάτωσης από τη [Γεννήτρια Widget](https://givelink.app/charities/widget-gen)
2. Προσθέστε ένα στοιχείο **Button** στη σελίδα σας και προσαρμόστε το
3. Ενεργοποιήστε τη **λειτουργία Dev**, επιλέξτε το κουμπί και ορίστε το ID του ως `givelink-button`
4. Προσθέστε τον παρακάτω κώδικα στον **Page Code**:
   ```javascript
   $w.onReady(function () {
     $w("#givelink-button").customClassList.add("givelink-button");
   });
   ```
5. Προσθέστε ένα στοιχείο **Custom Code** (body start) και επικολλήστε τον κώδικα ενσωμάτωσης
6. Αποθηκεύστε και δημοσιεύστε

📖 [Πλήρης Οδηγός Wix →](../en/iframe/wix.md)

---

### Προσαρμοσμένη Ιστοσελίδα (HTML/JavaScript)

1. Αντιγράψτε τον κώδικα ενσωμάτωσης από τη [Γεννήτρια Widget](https://givelink.app/charities/widget-gen)
2. Επικολλήστε τον κώδικα στο HTML σας (π.χ. πριν το `</body>`)
3. Προσθέστε ένα κουμπί με την κλάση `givelink-button`:
   ```html
   <button class="givelink-button">Δείτε τις Ανάγκες μας</button>
   ```
4. Αναπτύξτε τις αλλαγές σας

📖 [Πλήρης Οδηγός Native JavaScript →](../en/iframe/native.md)

---

## Επιλογή Β – Ενσωματωμένο Widget

Το widget εμφανίζεται απευθείας στη σελίδα — χωρίς να χρειάζεται κλικ σε κάποιο κουμπί. Οι επισκέπτες βλέπουν αμέσως το widget δωρεών όταν επισκέπτονται τη σελίδα.

**Οργανισμοί που χρησιμοποιούν αυτή την επιλογή:** BOSS

### WordPress

1. Στη [Γεννήτρια Widget](https://givelink.app/charities/widget-gen), επιλέξτε την καρτέλα **Inline** και αντιγράψτε τον κώδικα
2. Στον επεξεργαστή WordPress, προσθέστε ένα μπλοκ **Custom HTML**
3. Επικολλήστε τον κώδικα ενσωμάτωσης inline στο μπλοκ
4. Αποθηκεύστε και δημοσιεύστε

---

### Squarespace

1. Στη [Γεννήτρια Widget](https://givelink.app/charities/widget-gen), επιλέξτε την καρτέλα **Inline** και αντιγράψτε τον κώδικα
2. Επεξεργαστείτε τη σελίδα σας και προσθέστε ένα μπλοκ **Code** εκεί που θέλετε να εμφανιστεί το widget
3. Επικολλήστε τον κώδικα inline στο μπλοκ
4. Αποθηκεύστε και δημοσιεύστε

---

### Wix

1. Στη [Γεννήτρια Widget](https://givelink.app/charities/widget-gen), επιλέξτε την καρτέλα **Inline** και αντιγράψτε τον κώδικα
2. Στον επεξεργαστή Wix, κάντε κλικ στο **Add Element → Embed → Embed HTML**
3. Επικολλήστε τον κώδικα inline και ρυθμίστε το μέγεθος ώστε να ταιριάζει στη διάταξη σας
4. Αποθηκεύστε και δημοσιεύστε

---

### Προσαρμοσμένη Ιστοσελίδα (HTML)

1. Στη [Γεννήτρια Widget](https://givelink.app/charities/widget-gen), επιλέξτε την καρτέλα **Inline** και αντιγράψτε τον κώδικα
2. Επικολλήστε τον απευθείας στο HTML σας, εκεί που θέλετε να εμφανιστεί το widget:
   ```html
   <!-- Επικολλήστε εδώ τον κώδικα Givelink inline ενσωμάτωσης -->
   ```
3. Αναπτύξτε τις αλλαγές σας

---

> 💡 **Συμβουλή:** Ο κώδικας inline ενσωμάτωσης (Επιλογή Β) είναι διαφορετικός από τον κώδικα αναδυόμενου παραθύρου (Επιλογή Α). Βεβαιωθείτε ότι επιλέγετε τη σωστή καρτέλα στη Γεννήτρια Widget.

---

📖 **[Επιστροφή στο Κέντρο Ενσωμάτωσης →](../en/iframe/landing.md)**
