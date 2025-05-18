<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Mahi Beauty Parlour</title>
  <meta name="description" content="Book your beauty services at Mahi Beauty Parlour in Rajkot. Facial, Haircut, Hair Spa & more." />
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: flex-start;
      padding: 40px 20px;
    }
    .container {
      background-color: white;
      width: 100%;
      max-width: 600px;
      border-radius: 15px;
      box-shadow: 0 8px 24px rgba(0,0,0,0.15);
      padding: 30px 40px;
      box-sizing: border-box;
    }
    header {
      text-align: center;
      margin-bottom: 30px;
    }
    header img {
      max-width: 180px;
      margin-bottom: 10px;
    }
    header .logo {
      font-family: 'Brush Script MT', cursive;
      font-size: 48px;
      color: #ee6c7b;
      font-weight: 700;
      letter-spacing: 3px;
      margin-bottom: 5px;
      text-shadow: 1px 1px 3px #b83245;
    }
    .address {
      font-size: 0.9em;
      color: #666;
      letter-spacing: 0.5px;
    }
    section.services {
      margin-bottom: 35px;
    }
    h2 {
      color: #ee6c7b;
      font-weight: 600;
      margin-bottom: 20px;
      border-bottom: 2px solid #ee9ca7;
      padding-bottom: 5px;
    }
    .service-item {
      display: flex;
      justify-content: space-between;
      background: #fff0f2;
      border-radius: 8px;
      padding: 12px 18px;
      margin-bottom: 12px;
      box-shadow: 0 3px 8px rgba(238,108,123,0.2);
      align-items: center;
      font-weight: 600;
      color: #ee6c7b;
      transition: transform 0.2s ease;
    }
    .service-item:hover {
      transform: translateX(5px);
      box-shadow: 0 5px 15px rgba(238,108,123,0.3);
    }
    .service-item button {
      background-color: #ee6c7b;
      border: none;
      color: white;
      padding: 8px 16px;
      border-radius: 25px;
      cursor: pointer;
      font-weight: 600;
      font-size: 0.9em;
      box-shadow: 0 4px 10px rgba(238,108,123,0.4);
      transition: background-color 0.3s ease;
    }
    .service-item button:hover {
      background-color: #d95465;
    }
    #booking-form {
      display: none;
      border-radius: 12px;
      padding: 25px 30px;
      background: #fff0f2;
      box-shadow: 0 6px 18px rgba(238,108,123,0.25);
      margin-bottom: 30px;
      font-weight: 600;
      color: #ee6c7b;
    }
    #booking-form h2 {
      margin-top: 0;
      margin-bottom: 20px;
      color: #b83245;
    }
    label {
      display: block;
      margin-bottom: 6px;
      font-weight: 600;
    }
    input, select, textarea {
      width: 100%;
      padding: 9px 12px;
      border-radius: 8px;
      border: 1.5px solid #ee9ca7;
      margin-bottom: 18px;
      font-size: 1em;
      color: #5a2e35;
      font-weight: 500;
      box-sizing: border-box;
      transition: border-color 0.3s ease;
    }
    input:focus, select:focus, textarea:focus {
      outline: none;
      border-color: #ee6c7b;
      background: #fff7f9;
    }
    textarea {
      resize: vertical;
      min-height: 70px;
    }
    button#submitBooking {
      background-color: #ee6c7b;
      color: white;
      border: none;
      padding: 12px 0;
      border-radius: 30px;
      font-weight: 700;
      font-size: 1.1em;
      cursor: pointer;
      width: 100%;
      box-shadow: 0 5px 18px rgba(238,108,123,0.5);
      transition: background-color 0.3s ease;
    }
    button#submitBooking:hover {
      background-color: #d95465;
    }
    button#closeBooking {
      background: #d95465;
      color: #fff;
      border: none;
      padding: 8px 16px;
      border-radius: 8px;
      cursor: pointer;
      margin-bottom: 20px;
      font-weight: 600;
      box-shadow: 0 4px 10px rgba(217,84,101,0.6);
      transition: background-color 0.3s ease;
    }
    button#closeBooking:hover {
      background-color: #b73244;
    }
    section.contact {
      border-top: 1px solid #ee9ca7;
      padding-top: 20px;
      font-size: 1em;
      color: #66343f;
    }
    section.contact h2 {
      color: #ee6c7b;
      margin-bottom: 15px;
    }
    .call-btn {
      background-color: #48c774;
      color: white;
      padding: 10px 22px;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      font-weight: 700;
      box-shadow: 0 4px 14px rgba(72,199,116,0.5);
      transition: background-color 0.3s ease;
      margin-bottom: 10px;
    }
    .call-btn:hover {
      background-color: #2b8a3e;
    }
    a {
      color: #b83245;
      text-decoration: none;
      font-weight: 600;
    }
    a:hover {
      text-decoration: underline;
    }
    .payment-info {
      margin-top: 20px;
      font-style: italic;
      color: #8b4754;
    }
    @media(max-width: 640px){
      .container {
        padding: 25px 20px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <img src="mahi-logo.png" alt="Mahi Beauty Salon Logo" />
      <div class="logo">Mahi Beauty Parlour</div>
      <div class="address">
        Street no.1, University Road, Munjaka, Rajkot
      </div>
    </header>

    <section class="services">
      <h2>Our Services</h2>
      <div class="service-item"><span>Facial</span><button onclick="openBookingForm('Facial')">Book Now</button></div>
      <div class="service-item"><span>Haircut</span><button onclick="openBookingForm('Haircut')">Book Now</button></div>
      <div class="service-item"><span>Hairstyle</span><button onclick="openBookingForm('Hairstyle')">Book Now</button></div>
      <div class="service-item"><span>Hair Spa</span><button onclick="openBookingForm('Hair Spa')">Book Now</button></div>
      <div class="service-item"><span>Eyebrow</span><button onclick="openBookingForm('Eyebrow')">Book Now</button></div>
      <div class="service-item"><span>Wax</span><button onclick="openBookingForm('Wax')">Book Now</button></div>
      <div class="service-item"><span>Skin Care</span><button onclick="openBookingForm('Skin Care')">Book Now</button></div>
      <div class="service-item"><span>Nail Art</span><button onclick="openBookingForm('Nail Art')">Book Now</button></div>
      <div class="service-item"><span>Mahendi</span><button onclick="openBookingForm('Mahendi')">Book Now</button></div>
    </section>

    <section id="booking-form" aria-label="Booking Form">
      <h2>Book Your Appointment</h2>
      <button id="closeBooking" type="button" onclick="closeBookingForm()">Close</button>
      <form id="appointmentForm" onsubmit="return submitBooking(event)" aria-describedby="booking-form">
        <label for="name">Name *</label>
        <input type="text" id="name" name="name" required aria-required="true" aria-label="Name" />
        <label for="phone">Phone Number *</label>
        <input type="tel" id="phone" name="phone" pattern="[0-9]{10}" placeholder="Enter 10-digit number" required aria-required="true" aria-label="Phone Number" />
        <label for="email">Email</label>
        <input type="email" id="email" name="email" placeholder="Optional" aria-label="Email" />
        <label for="service">Service *</label>
        <input type="text" id="service" name="service" readonly aria-readonly="true" aria-label="Service" />
        <label for="date">Select Date *</label>
        <input type="date" id="date" name="date" required aria-required="true" aria-label="Select Date" />
        <label for="time">Select Time *</label>
        <input type="time" id="time" name="time" required aria-required="true" aria-label="Select Time" />
        <label for="notes">Special Requests</label>
        <textarea id="notes" name="notes" rows="3" placeholder="Any special requirements" aria-label="Special Requests"></textarea>
        <button type="submit" id="submitBooking">Confirm Booking</button>
      </form>
    </section>

    <section class="contact">
      <h2>Contact Us</h2>
      <p>Phone: <a href="tel:+919316471580">+91 9316471580</a></p>
      <a href="tel:+919316471580"><button class="call-btn">Call Now</button></a>
      <p>Email: <a href="mailto:mahibeatysalon47@gmail.com">mahibeatysalon47@gmail.com</a></p>
      <p>Instagram: <a href="https://instagram.com/mahi_beauty_salon_7" target="_blank" rel="noopener noreferrer">@mahi_beauty_salon_7</a></p>
      <div class="payment-info">
        Payment options will be available after booking confirmation.
      </div>
    </section>
  </div>

  <script>
    // Set minimum date to today to avoid past date booking
    window.onload = () => {
      const dateInput = document.getElementById('date');
      const today = new Date().toISOString().split('T')[0];
      dateInput.min = today;
    };

    function openBookingForm(service) {
      document.getElementById('booking-form').style.display = 'block';
      document.getElementById('service').value = service;
      window.scrollTo({ top: document.body.scrollHeight, behavior: 'smooth' });
    }

    function closeBookingForm() {
      document.getElementById('booking-form').style.display = 'none';
    }

    function submitBooking(event) {
      event.preventDefault();
      const form = document.getElementById('appointmentForm');
      const formData = new FormData(form);

      // Validate phone length as extra check
      const phone = formData.get('phone');
      if (!/^\d{10}$/.test(phone)) {
        alert('Please enter a valid 10-digit phone number.');
        return false;
      }

      alert(
        'Booking Confirmed!\n' +
        'Name: ' + formData.get
        ('name') + '\n' +
        'Phone: ' + phone + '\n' +
        'Email: ' + formData.get('email') + '\n' +
        'Service: ' + formData.get('service') + '\n' +
        'Date: ' + formData.get('date') + '\n' +
        'Time: ' + formData.get('time') + '\n' +
        'Notes: ' + formData.get('notes')
      );
      form.reset();
      document.getElementById('booking-form').style.display = 'none';
      return false;
    }
  </script>
</body>
</html
