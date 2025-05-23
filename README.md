# tensorflow
Neural network training for handwritten numeral digit recognition

---

## Στόχος της Εργασίας

Στόχος της εργασίας είναι η εκπαίδευση Βαθιών Νευρωνικών Δικτύων (Deep Neural Networks) για την ταξινόμηση (Classification) χειρόγραφων ψηφίων (0-9).

## Υλοποίηση

- Τα δεδομένα του MINST φορτώθηκαν με τη χρήση του TensorFlow.
- Οι εικόνες των 28x28 pixels μετατράπηκαν σε διανύσματα μεγέθους 784 ενώ οι ετικέτες κωδικοποιήθηκαν με one-hot encoding.
- Το αρχικό δίκτυο αποτελείται από ένα επίπεδο εισόδου με 784 νευρώνες, δύο κρυφά επίπεδα με 256 νευρώνες το καθένα και συνάρτηση ενεργοποίησης tanh, και ένα επίπεδο εξόδου με 10 νευρώνες και softmax ενεργοποίηση.
- Χρησιμοποιήθηκε η βελτιστοποίηση Stochastic Gradient Descent (SGD) με ρυθμό μάθησης 0.001.
- Εκπαιδεύτηκε για 10 εποχές.
- Δοκιμάστηκε η βελτιστοποίηση της απόδοσης μέσω παραμετροποίησης
	- στα επίπεδα,
	- τον αριθμό των νευρώνων,
	- τις εποχές,
	- το ρυθμό μάθησης και
	- τη συνάρτηση ενεργοποίησης.
- Εφαρμόστηκε dropout 0.3 στα κρυφά επίπεδα, χωρίς όμως αυτό να επιφέρει βελτίωση στην ακρίβεια.
- Για κάθε μοντέλο υπολογίστηκε η ακρίβεια και το σφάλμα κατά την εκπαίδευση και την επικύρωση.

## Αποτελέσματα

Η ακρίβεια του τελικού μοντέλου πέτυχε ακρίβεια πάνω από 95% στα δεδομένα δοκιμής, συνεπώς το Νευρωνικό Δίκτυο είναι απολύτως ικανό να χρησιμοποιηθεί στην αναγνώριση χειρόγραφων ψηφίων.

---

*Λευκόπουλος Γεώργιος (4588) | Τμήμα Πληροφορικής | Σ.Θ.Ε. | Α.Π.Θ.*
