# Ενσωμάτωση Wix

Ακολουθήστε τα παρακάτω βήματα:

1. Αντιγράψτε τον κωδικό HTML <strong>επιλέγοντας</strong> τον μη κερδοσκοπικό οργανισμό που θέλετε να προωθήσετε από τη [Σελίδα Αντιγραφής Widget](https://givelink.app/charities/widget-gen)

   ![Αντιγραφή Κωδικού](/assets/widget-assets-greek.png)

2. Μεταβείτε στον πίνακα επεξεργασίας Wix.
3. Πλοηγηθείτε στο `Website & mobile app > Website`, πατήστε edit site επάνω δεξιά

4. Επιλέξτε Add Element επάνω αριστερά, στη συνέχεια Button

![Προσθήκη Κουμπιού](/assets/wix/wix_add_button.png)

5. Τοποθετήστε το κουμπί στη σελίδα. Μπορείτε ελεύθερα να προσαρμόσετε χρώματα και γραμματοσειρά σύμφωνα με τον ιστότοπό σας. Βεβαιωθείτε ότι η Παρότρυνση για Δράση είναι <strong>"Δώρισε σε είδος"</strong>, <strong>"Δες τις ανάγκες μας"</strong> ή κάτι παρόμοιο.

6. Από τη γραμμή επάνω, ενεργοποιήστε τη λειτουργία Dev Mode, στη συνέχεια επιλέξτε το κουμπί που μόλις δημιουργήσατε και προσθέστε ως id: `givelink-button`

![Dev Mode](/assets/wix/dev_mode.png)

7. Προσθέστε τον παρακάτω κώδικα στον κώδικα σελίδας:

```javascript
$w.onReady(function () {
  $w("#givelink-button").customClassList.add("givelink-button");
});
```

![Velo Code](/assets/wix/velo_code.png)

8. Κάντε κλικ στο add element και αναζητήστε Custom code

![Στοιχείο Custom code](/assets/wix/custom_code_element.png)

9. Προσθέστε σε ένα νέο στοιχείο Custom code στην ενότητα body start, επικολλήστε τον κώδικα που αντιγράψατε στο βήμα 1 και πατήστε apply.

![Σελίδα Custom code](/assets/wix/custom_code_page.png)

![Προσθήκη Κώδικα](/assets/wix/add_code.png)

10. Αποθηκεύστε και δημοσιεύστε τον ιστότοπό σας όταν είστε έτοιμοι.
