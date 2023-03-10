# Blue-Drop
Η εξάντληση των υδάτινων πόρων εξαιτίας της ανθρώπινης δραστηριότητας αποτελεί ένα από τα μεγαλύτερα προβλήματα της σύγχρονης κοινωνίας. Για αυτόν τον λόγο αποφασίσαμε να δημιουργήσουμε εναν υδρομετρητή ο οποίος θα μετράει την κατανάλωση του νερού σε λίτρα και θα αποστέλλει κατάλληλες ενδείξεις με στόχο την μείωση της σπατάλης νερού.

# ΑΝΑΛΥΤΙΚΗ ΠΕΡΙΓΡΑΦΗ ΙΔΕΑΣ:

Η εξάντληση των υδάτινων πόρων εξαιτίας της ανθρώπινης δραστηριότητας αποτελεί ένα από τα μεγαλύτερα προβλήματα της σύγχρονης κοινωνίας. Η υπέρμετρη κατανάλωση του νερού, δίχως αυτό να προσμετράται ή να κοστολογείται, αποτελεί τον κύριο παράγοντα του προβλήματος. Για αυτόν τον λόγο αποφασίσαμε να δημιουργήσουμε εναν υδρομετρητή ο οποίος θα μετράει την κατανάλωση του νερού σε λίτρα. Αν η μέτρηση αυτή ξεπερνάει τα προβλεπόμενα όρια σύμφωνα με τα προσωπικά δεδομένα του καταναλωτή, τότε μία ένδειξη ενεργοποιείται στη συσκευή και αποστέλλεται μήνυμα στο κινητό με τα δεδομένα της μέτρησης.

Η μείωση της σπατάλης νερού είναι σημαντική για τη διατήρηση των υδάτινων πόρων και τη μείωση των περιβαλλοντικών επιπτώσεων της χρήσης του νερού. Αυτό μπορεί να επιτευχθεί με την εφαρμογή τεχνολογιών και πρακτικών εξοικονόμησης νερού,

Στην σημερινή κοινωνία η αλόγιστη σπατάλη του νερού αποτελεί ένα μείζον θέμα στην εποχή μας.

Περίπου το 95% του νερού που εισέρχεται στα σπίτια καταλήγει στον υπόνομο
Αφήνοντας ανοιχτή τη βρύση ενώ βουρτσίζετε τα δόντια σας είναι σαν να ρίχνετε περίπου 15 λίτρα νερού στον νεροχύτη
Οι χαλασμένες βρύσες που στάζουν ανά δευτερόλεπτο μπορούν να σπαταλήσουν έως και 10.220 λίτρα νερού κάθε χρόνο.
Ενα μικρό πλυντήριο πιάτων θα χρειαστεί περίπου 15 λίτρα νερό ανά πλύση


Συγκεκριμενα, αποφασισαμε να δημιουργησουμε μια συσκευή η οποία θα συνδέεται στο στόμιο της βρύσης και σε άλλους τέτοιου τύπου σωλήνες. Ουσιαστικά η συσκευή περιλαμβάνει μια προπέλα που τίθεται σε κίνηση λόγω της ροής του νερού μέσα στο σωλήνα. Η ενέργεια που θα παραγει η κίνηση αυτή θα εξυπηρετεί στην λειτουργία ενός arduino– ESP8266. Το arduino θα μετρά την ενέργεια που παράγει η κίνηση της προπέλας και με μία αντιστοιχία θα υπολογίζει την ποσότητα του νερού που πέρασε. Αν αυτος ο αριθμος ξεπερνάει ένα προκαθορισμένο όριο το arduino θα στελνει μηνυμα μεσω εφαρμογής και θα ενημερώνει τον χρήστη για την υπερκατανάλωση. 

Την συσκευή αυτή σκεφτόμαστε στο μέλλον να την εξελίξουμε ούτως ώστε να μπορεί να τοποθετηθεί σε όλες τις συσκευές που καταναλώνουν νερό (π.χ. βρύσες, σωλήνες) είτε μέσω ενός φίλτρου που θα μπορεί να μπαίνει στην άκρη της βρύσης είτε μέσου ενός παρόμοιου συστηματος σε σωλήνες. Μάλιστα, στα καινούργια σπίτια, εργοστάσια, χώρους εργασίας, σχολεία θα είναι ακόμη ευκολότερη η εγκατάσταση της συσκευής μας μέσα στους καινούργιους σωλήνες οι οποίοι θα αποτελούν την κύρια παροχή νερού του κτίσματος ούτως ώστε να μην χρειάζεται να μπει σε όλες τις βρύσες και γενικότερα στα μέσα κατανάλωσης τους νερού.


# ΣΧΕΔΙΑΣΜΟΣ ΙΔΕΑΣ:

Σκεφτηκαμε να φτιάξουμε ένα ροόμετρο που θα μετράει την κατανάλωση του νερού μέσα σε ένα τμήμα σωλήνα. Πιο συγκεκριμένα μέσα στο σωλήνα θα βρισκεται μια προπέλα η οποία θα περιστρέφεται και θα παράγει ενέργεια ανάλογη της ποσότητας του νερού που την διαπερνά (δηλαδή, ανάλογη των περιστροφών της προπέλας). Αυτο το σύστημα θα συνδέεται με ενα arduino esp8266, το οποίο με τις δυνατότητες που προσφέρει μέσω του διαδικτύου των πραγμάτων, θα στέλνει τα δεδομένα που έχει συλλέξει απευθείας στο τηλέφωνο του χρήστη. Ομως για να βρουμε την ακριβη ποσοτητα που θα χρειαστει για να γίνεται η σωστή μέτρηση της κατανάλωσης, καθίσταται απαραίτητο να γίνει έρευνα στον ακριβή αριθμό ενέργειας που παράγεται ανα λιτρο. Όταν αυτος ο αριθμος προσδιοριστει τότε ανάλογα με την ενεργεια που παραγεται θα μπορουμε να βρουμε τη συνολικη ποσότητα νερού που έχει καταναλωθει. 


# ΥΛΙΚΑ ΠΟΥ ΘΑ ΧΡΗΣΙΜΟΠΟΙΗΘΟΥΝ:

Για την κατασκευη του μετρητή νερού (ροομέτρου) θα χρειαστούμε:
- Τμημα σωληνα
- Καλωδια
- Προπέλα μικρού μεγέθους 
- Πολύμετρο  
- Arduino uno
- esp8266
- Μικρού μεγέθους inverter
