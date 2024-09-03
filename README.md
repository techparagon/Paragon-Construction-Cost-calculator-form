## Requirements

### 1) Προσθήκη του παρακάτω κώδικα στο functions.php του theme
function mytheme_enqueue_styles() {
	// Enqueue Bootstrap CSS from jsDelivr CDN
	wp_enqueue_style('bootstrap-css', 'https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css');
}

add_action('wp_enqueue_scripts', 'mytheme_enqueue_styles');

### 2 Δημιουργούμε ένα shortcode στο functions.php και περνάμε μέσα τον κώδικα από το αρχείο Cost Calculator.html
