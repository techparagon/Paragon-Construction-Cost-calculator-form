## Requirements & How to use

### 1) Προσθήκη του παρακάτω κώδικα στο functions.php του theme
function mytheme_enqueue_styles() {
	// Enqueue Bootstrap CSS from jsDelivr CDN
	wp_enqueue_style('bootstrap-css', 'https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css');
}

add_action('wp_enqueue_scripts', 'mytheme_enqueue_styles');

### 2 Δημιουργούμε ένα shortcode στο functions.php και περνάμε μέσα τον κώδικα από το αρχείο Cost Calculator.html
### 3 Δημιουργούμε μια φόρμα επικοινωνίας και εισάγουμε στα αντίστοιχα πεδία της το περιεχόμενο από τα αρχεία Contact form Πεδίο Φόρμας.html και Contact form Πεδίο Αλληλογραφίας.html
### 4 Εισάγουμε τον κώδικα CSS στο wordpress customizer (Προσαρμογή από το μενού)
### 5 Σημαντικό μέσα στο κώδικα CSS αλλάζουμε την κλάση .page-id-6188 στο id της νέας μας σελίδας
### 6 Εισάγουμε τα shortcode της φόρμας και του κώδικα που φτιάξαμε στο βήμα 1 στην σελίδα που επιθυμούμε
Παραδειγμα: 
[my_cost_form]
[contact-form-7 id="6028" title="Φόρμα υπολογισμός κόστους ανακαίνισης"]
