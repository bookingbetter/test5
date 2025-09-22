<!DOCTYPE html>
<html lang="el">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BookingBetter</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    /* Reset & βασικά styles */
    * { margin:0; padding:0; box-sizing:border-box; font-family: 'Montserrat', sans-serif;}
    body {line-height:1.6; color:#333;}
    a {text-decoration:none; color:inherit;}
    img {max-width:100%; display:block;}

    /* Header */
    header {display:flex; justify-content:space-between; align-items:center; padding:20px 10%; background:#0D6EFD; color:white; position:sticky; top:0; z-index:1000;}
    header .logo {font-size:1.5rem; font-weight:700;}
    nav a {margin-left:20px; font-weight:600; transition:0.3s;}
    nav a:hover {color:#FFC107;}

    /* Hero Section */
    .hero {height:90vh; background:linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://source.unsplash.com/1600x900/?hotel,travel') center/cover no-repeat; display:flex; flex-direction:column; justify-content:center; align-items:center; text-align:center; color:white;}
    .hero h1 {font-size:3rem; margin-bottom:20px;}
    .hero p {font-size:1.5rem; margin-bottom:30px;}
    .hero a {padding:15px 30px; background:#FFC107; color:#333; font-weight:700; border-radius:5px; transition:0.3s;}
    .hero a:hover {background:#FFD633;}

    /* Υπηρεσίες */
    .services {padding:80px 10%; display:flex; flex-wrap:wrap; justify-content:space-between; gap:30px;}
    .service {flex:1 1 300px; padding:20px; border-radius:10px; background:#f5f5f5; text-align:center; transition:0.3s;}
    .service:hover {transform:translateY(-10px); box-shadow:0 10px 20px rgba(0,0,0,0.1);}
    .service h3 {margin-bottom:15px; color:#0D6EFD;}
    .service p {color:#555;}

    /* Γιατί εμάς */
    .why {background:#e9ecef; padding:80px 10%; text-align:center;}
    .why h2 {margin-bottom:40px; color:#0D6EFD;}
    .points {display:flex; flex-wrap:wrap; justify-content:space-between; gap:30px;}
    .point {flex:1 1 250px; background:white; padding:30px; border-radius:10px; transition:0.3s;}
    .point:hover {transform:translateY(-10px); box-shadow:0 10px 20px rgba(0,0,0,0.1);}
    .point h3 {margin-bottom:10px;}
    .point p {color:#555;}

    /* Επικοινωνία */
    .contact {padding:80px 10%; text-align:center;}
    .contact h2 {margin-bottom:40px; color:#0D6EFD;}
    form {max-width:600px; margin:0 auto; display:flex; flex-direction:column; gap:20px;}
    input, textarea {padding:15px; border-radius:5px; border:1px solid #ccc; font-size:1rem; width:100%;}
    button {padding:15px; border:none; border-radius:5px; background:#0D6EFD; color:white; font-weight:700; cursor:pointer; transition:0.3s;}
    button:hover {background:#0056b3;}

    /* Footer */
    footer {padding:40px 10%; background:#333; color:white; text-align:center;}
    footer a {color:#FFC107; margin:0 10px; transition:0.3s;}
    footer a:hover {color:#FFD633;}

    /* Responsive */
    @media(max-width:768px) {
      header {flex-direction:column;}
      nav a {margin:10px;}
      .services, .points {flex-direction:column; align-items:center;}
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="logo">BookingBetter</div>
    <nav>
      <a href="#hero">Home</a>
      <a href="#services">Υπηρεσίες</a>
      <a href="#why">Γιατί εμάς</a>
      <a href="#contact">Επικοινωνία</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero" id="hero">
    <h1>Η πρώτη εντύπωση φέρνει την κράτηση</h1>
    <p>Βελτιστοποιούμε την παρουσία σας στο Booking και σε άλλες πλατφόρμες</p>
    <a href="#services">Δες τις υπηρεσίες μας</a>
  </section>

  <!-- Services -->
  <section class="services" id="services">
    <div class="service">
      <h3>Φωτογράφιση καταλυμάτων</h3>
      <p>Υψηλής ποιότητας φωτογραφίες που αναδεικνύουν τον χώρο σας.</p>
    </div>
    <div class="service">
      <h3>Βελτιωμένες περιγραφές</h3>
      <p>Σαφείς και πιασάρικες περιγραφές που αυξάνουν το ενδιαφέρον των επισκεπτών.</p>
    </div>
    <div class="service">
      <h3>Διαχείριση καταχώρησης</h3>
      <p>Ακριβής και ελκυστική παρουσίαση στα Booking, Airbnb και άλλες πλατφόρμες.</p>
    </div>
  </section>

  <!-- Why Us -->
  <section class="why" id="why">
    <h2>Γιατί να επιλέξετε εμάς</h2>
    <div class="points">
      <div class="point">
        <h3>Επαγγελματισμός</h3>
        <p>Προσφέρουμε υπηρεσίες υψηλής ποιότητας και αξιοπιστίας.</p>
      </div>
      <div class="point">
        <h3>Εμπειρία</h3>
        <p>Γνωρίζουμε τι χρειάζεται για να ξεχωρίσει η καταχώρησή σας.</p>
      </div>
      <div class="point">
        <h3>Αποτελέσματα</h3>
        <p>Αυξάνουμε την ορατότητα και τις κρατήσεις σας.</p>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section class="contact" id="contact">
    <h2>Επικοινωνήστε μαζί μας</h2>
    <form id="contactForm">
      <input type="text" name="name" placeholder="Όνομα" required>
      <input type="email" name="email" placeholder="Email" required>
      <textarea name="message" placeholder="Μήνυμα" rows="5" required></textarea>
      <button type="submit">Αποστολή</button>
    </form>
    <p id="formMessage" style="margin-top:15px; color:green;"></p>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2025 BookingBetter. Όλα τα δικαιώματα διατηρούνται.</p>
    <p>
      <a href="#">Facebook</a>|
      <a href="#">Instagram</a>|
      <a href="#">LinkedIn</a>
    </p>
  </footer>

  <script>
    // Φόρμα επικοινωνίας
    const form = document.getElementById('contactForm');
    const formMessage = document.getElementById('formMessage');

    form.addEventListener('submit', function(e){
      e.preventDefault();
      formMessage.textContent = 'Το μήνυμά σας στάλθηκε επιτυχώς! Ευχαριστούμε.';
      form.reset();
    });
  </script>

</body>
</html>
