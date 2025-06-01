<html lang="en">
 <head>
  <meta charset="utf-8"/>
  <meta content="width=device-width, initial-scale=1" name="viewport"/>
  <title>
   OYO Clone - Hotel Booking
  </title>
  <script src="https://cdn.tailwindcss.com">
  </script>
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&amp;display=swap" rel="stylesheet"/>
  <style>
   body {
      font-family: 'Montserrat', sans-serif;
    }
  </style>
 </head>
 <body class="bg-gray-50">
  <!-- Header / Navbar -->
  <header class="bg-white shadow-md sticky top-0 z-50">
   <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-16">
     <a class="flex items-center space-x-2" href="#">
      <img alt="OYO logo red square with white OYO text" class="h-10 w-10 rounded" height="48" src="https://storage.googleapis.com/a1aa/image/69c56f9f-f62b-4057-93ce-e51dec244e81.jpg" width="48"/>
      <span class="text-2xl font-bold text-red-600">
       OYO
      </span>
     </a>
     <nav class="hidden md:flex space-x-8 font-semibold text-gray-700">
      <a class="hover:text-red-600 transition" href="#">
       Stays
      </a>
      <a class="hover:text-red-600 transition" href="#">
       OYO Wizard
      </a>
      <a class="hover:text-red-600 transition" href="#">
       OYO Workspaces
      </a>
      <a class="hover:text-red-600 transition" href="#">
       Offers
      </a>
      <a class="hover:text-red-600 transition" href="#">
       Help
      </a>
     </nav>
     <div class="hidden md:flex items-center space-x-4">
      <button id="login-button" class="text-gray-700 hover:text-red-600 transition font-semibold">
       Login
      </button>
      <button id="signup-button" class="bg-red-600 text-white px-4 py-2 rounded-md font-semibold hover:bg-red-700 transition">
       Sign Up
      </button>
     </div>
     <button aria-label="Open menu" class="md:hidden text-gray-700 hover:text-red-600 focus:outline-none" id="mobile-menu-button">
      <i class="fas fa-bars fa-lg">
      </i>
     </button>
    </div>
   </div>
   <!-- Mobile menu -->
   <div class="md:hidden hidden bg-white border-t border-gray-200" id="mobile-menu">
    <nav class="flex flex-col space-y-1 p-4 font-semibold text-gray-700">
     <a class="hover:text-red-600 transition" href="#">
      Stays
     </a>
     <a class="hover:text-red-600 transition" href="#">
      OYO Wizard
     </a>
     <a class="hover:text-red-600 transition" href="#">
      OYO Workspaces
     </a>
     <a class="hover:text-red-600 transition" href="#">
      Offers
     </a>
     <a class="hover:text-red-600 transition" href="#">
      Help
     </a>
     <button id="mobile-login-button" class="text-left text-gray-700 hover:text-red-600 transition font-semibold mt-2">
      Login
     </button>
     <button id="mobile-signup-button" class="bg-red-600 text-white px-4 py-2 rounded-md font-semibold hover:bg-red-700 transition mt-2">
      Sign Up
     </button>
    </nav>
   </div>
  </header>
  <!-- Hero Section -->
  <section class="relative bg-red-600 text-white">
   <img alt="Beautiful hotel lobby with modern design and warm lighting, spacious seating area with plants and ambient lights" class="w-full h-60 sm:h-96 object-cover brightness-75" height="600" src="https://storage.googleapis.com/a1aa/image/3be3c7fe-3f06-4296-c318-3711f58d2c2d.jpg" width="1920"/>
   <div class="absolute inset-0 flex flex-col justify-center items-center px-4 sm:px-6 lg:px-8">
    <h1 class="text-3xl sm:text-5xl font-extrabold mb-4 text-center max-w-4xl">
     Find and Book Your Perfect Stay
    </h1>
    <p class="text-lg sm:text-xl mb-8 text-center max-w-3xl">
     Explore thousands of hotels, homes, and stays worldwide at unbeatable
        prices.
    </p>
    <form aria-label="Search hotels form" class="bg-white rounded-md shadow-lg p-4 sm:p-6 flex flex-col sm:flex-row items-center max-w-4xl w-full">
     <div class="flex-1 w-full sm:mr-4 mb-4 sm:mb-0">
      <label class="sr-only" for="location">
       Location
      </label>
      <input class="w-full border border-gray-300 rounded-md px-4 py-3 focus:outline-none focus:ring-2 focus:ring-red-600" id="location" name="location" placeholder="Enter city or hotel name" type="text"/>
     </div>
     <div class="flex-1 w-full sm:mr-4 mb-4 sm:mb-0 grid grid-cols-2 gap-4">
      <div>
       <label class="sr-only" for="checkin">
        Check-in date
       </label>
       <input class="w-full border border-gray-300 rounded-md px-4 py-3 focus:outline-none focus:ring-2 focus:ring-red-600" id="checkin" name="checkin" type="date"/>
      </div>
      <div>
       <label class="sr-only" for="checkout">
        Check-out date
       </label>
       <input class="w-full border border-gray-300 rounded-md px-4 py-3 focus:outline-none focus:ring-2 focus:ring-red-600" id="checkout" name="checkout" type="date"/>
      </div>
     </div>
     <div class="flex-1 w-full sm:mr-4 mb-4 sm:mb-0">
      <label class="sr-only" for="guests">
       Guests
      </label>
      <select class="w-full border border-gray-300 rounded-md px-4 py-3 focus:outline-none focus:ring-2 focus:ring-red-600" id="guests" name="guests">
       <option value="1">
        1 Guest
       </option>
       <option value="2">
        2 Guests
       </option>
       <option value="3">
        3 Guests
       </option>
       <option value="4">
        4 Guests
       </option>
       <option value="5">
        5 Guests
       </option>
       <option value="6">
        6 Guests
       </option>
       <option value="7">
        7 Guests
       </option>
       <option value="8">
        8 Guests
       </option>
      </select>
     </div>
     <button class="bg-red-600 hover:bg-red-700 text-white font-semibold rounded-md px-6 py-3 w-full sm:w-auto transition" type="submit">
      Search
     </button>
    </form>
   </div>
  </section>
  <!-- Popular Destinations -->
  <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
   <h2 class="text-3xl font-bold text-gray-900 mb-8 text-center">
    Popular Destinations
   </h2>
   <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-6">
    <a class="group block rounded-lg overflow-hidden shadow-lg hover:shadow-2xl transition" href="#">
     <img alt="New York City skyline at sunset with tall skyscrapers and orange sky" class="w-full h-48 object-cover group-hover:scale-105 transition-transform duration-300" height="300" src="https://storage.googleapis.com/a1aa/image/a542ae2e-8265-4543-2dee-6acfc1fe804a.jpg" width="400"/>
     <div class="p-4 bg-white">
      <h3 class="text-lg font-semibold text-gray-900">
       New York City
      </h3>
      <p class="text-red-600 font-semibold mt-1">
       From $50/night
      </p>
     </div>
    </a>
    <a class="group block rounded-lg overflow-hidden shadow-lg hover:shadow-2xl transition" href="#">
     <img alt="Beach resort in Goa with palm trees, white sand beach and turquoise water" class="w-full h-48 object-cover group-hover:scale-105 transition-transform duration-300" height="300" src="https://storage.googleapis.com/a1aa/image/f5f579ae-fafd-4853-d88f-f485027fec7c.jpg" width="400"/>
     <div class="p-4 bg-white">
      <h3 class="text-lg font-semibold text-gray-900">
       Goa
      </h3>
      <p class="text-red-600 font-semibold mt-1">
       From $30/night
      </p>
     </div>
    </a>
    <a class="group block rounded-lg overflow-hidden shadow-lg hover:shadow-2xl transition" href="#">
     <img alt="Paris Eiffel Tower at night illuminated with city lights and dark blue sky" class="w-full h-48 object-cover group-hover:scale-105 transition-transform duration-300" height="300" src="https://storage.googleapis.com/a1aa/image/66f3f0c4-fa27-4e5f-234a-feac22e6ff59.jpg" width="400"/>
     <div class="p-4 bg-white">
      <h3 class="text-lg font-semibold text-gray-900">
       Paris
      </h3>
      <p class="text-red-600 font-semibold mt-1">
       From $70/night
      </p>
     </div>
    </a>
    <a class="group block rounded-lg overflow-hidden shadow-lg hover:shadow-2xl transition" href="#">
     <img alt="Tokyo cityscape with cherry blossoms in full bloom and modern buildings" class="w-full h-48 object-cover group-hover:scale-105 transition-transform duration-300" height="300" src="https://storage.googleapis.com/a1aa/image/745cc842-f176-4d90-32a2-e9f794a344d5.jpg" width="400"/>
     <div class="p-4 bg-white">
      <h3 class="text-lg font-semibold text-gray-900">
       Tokyo
      </h3>
      <p class="text-red-600 font-semibold mt-1">
       From $60/night
      </p>
     </div>
    </a>
   </div>
  </section>
  <!-- Featured Hotels -->
  <section class="bg-white py-12">
   <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <h2 class="text-3xl font-bold text-gray-900 mb-8 text-center">
     Featured Hotels
    </h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8">
     <article class="bg-gray-100 rounded-lg shadow-md overflow-hidden hover:shadow-xl transition">
      <img alt="Modern hotel room with king size bed, white linens, city view from window" class="w-full h-48 object-cover" height="250" src="https://storage.googleapis.com/a1aa/image/727f3ab6-00cb-494f-e673-c91ca62d8543.jpg" width="400"/>
      <div class="p-4">
       <h3 class="text-lg font-semibold text-gray-900 mb-1">
        The Grand Palace Hotel
       </h3>
       <p class="text-gray-700 mb-2">
        New York City, USA
       </p>
       <div class="flex items-center justify-between">
        <span class="text-red-600 font-bold text-lg">
         $120/night
        </span>
        <div class="flex items-center text-yellow-400">
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star-half-alt">
         </i>
         <span class="text-gray-600 ml-2 text-sm">
          (4.5)
         </span>
        </div>
       </div>
      </div>
     </article>
     <article class="bg-gray-100 rounded-lg shadow-md overflow-hidden hover:shadow-xl transition">
      <img alt="Cozy beachfront hotel room with balcony overlooking ocean and palm trees" class="w-full h-48 object-cover" height="250" src="https://storage.googleapis.com/a1aa/image/88ec27c0-9198-4ca6-ba8e-69d6d8829c1c.jpg" width="400"/>
      <div class="p-4">
       <h3 class="text-lg font-semibold text-gray-900 mb-1">
        Ocean Breeze Resort
       </h3>
       <p class="text-gray-700 mb-2">
        Goa, India
       </p>
       <div class="flex items-center justify-between">
        <span class="text-red-600 font-bold text-lg">
         $80/night
        </span>
        <div class="flex items-center text-yellow-400">
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star-half-alt">
         </i>
         <i class="far fa-star">
         </i>
         <span class="text-gray-600 ml-2 text-sm">
          (3.8)
         </span>
        </div>
       </div>
      </div>
     </article>
     <article class="bg-gray-100 rounded-lg shadow-md overflow-hidden hover:shadow-xl transition">
      <img alt="Luxury hotel suite with elegant decor, large windows and plush furniture" class="w-full h-48 object-cover" height="250" src="https://storage.googleapis.com/a1aa/image/dae0b4e9-7236-4b72-773f-2c248af99e60.jpg" width="400"/>
      <div class="p-4">
       <h3 class="text-lg font-semibold text-gray-900 mb-1">
        Parisian Elegance Hotel
       </h3>
       <p class="text-gray-700 mb-2">
        Paris, France
       </p>
       <div class="flex items-center justify-between">
        <span class="text-red-600 font-bold text-lg">
         $150/night
        </span>
        <div class="flex items-center text-yellow-400">
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <span class="text-gray-600 ml-2 text-sm">
          (5.0)
         </span>
        </div>
       </div>
      </div>
     </article>
     <article class="bg-gray-100 rounded-lg shadow-md overflow-hidden hover:shadow-xl transition">
      <img alt="Contemporary hotel room with city lights view at night, modern furniture" class="w-full h-48 object-cover" height="250" src="https://storage.googleapis.com/a1aa/image/9a246228-8fb6-483a-5e15-6500b5a7e54d.jpg" width="400"/>
      <div class="p-4">
       <h3 class="text-lg font-semibold text-gray-900 mb-1">
        Tokyo Skyline Hotel
       </h3>
       <p class="text-gray-700 mb-2">
        Tokyo, Japan
       </p>
       <div class="flex items-center justify-between">
        <span class="text-red-600 font-bold text-lg">
         $110/night
        </span>
        <div class="flex items-center text-yellow-400">
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star">
         </i>
         <i class="fas fa-star-half-alt">
         </i>
         <i class="far fa-star">
         </i>
         <span class="text-gray-600 ml-2 text-sm">
          (3.9)
         </span>
        </div>
       </div>
      </div>
     </article>
    </div>
   </div>
  </section>
  <!-- Why Choose OYO Section -->
  <section class="bg-red-50 py-12">
   <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
    <h2 class="text-3xl font-bold text-gray-900 mb-8">
     Why Choose OYO?
    </h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-8">
     <div class="bg-white rounded-lg shadow p-6 flex flex-col items-center">
      <i class="fas fa-bed fa-3x text-red-600 mb-4">
      </i>
      <h3 class="text-xl font-semibold mb-2">
       Wide Range of Stays
      </h3>
      <p class="text-gray-700">
       Choose from thousands of hotels, homes, and unique stays worldwide.
      </p>
     </div>
     <div class="bg-white rounded-lg shadow p-6 flex flex-col items-center">
      <i class="fas fa-tags fa-3x text-red-600 mb-4">
      </i>
      <h3 class="text-xl font-semibold mb-2">
       Best Price Guarantee
      </h3>
      <p class="text-gray-700">
       Get the best deals and discounts on your bookings every time.
      </p>
     </div>
     <div class="bg-white rounded-lg shadow p-6 flex flex-col items-center">
      <i class="fas fa-headset fa-3x text-red-600 mb-4">
      </i>
      <h3 class="text-xl font-semibold mb-2">
       24/7 Customer Support
      </h3>
      <p class="text-gray-700">
       Our support team is always ready to help you with your bookings.
      </p>
     </div>
     <div class="bg-white rounded-lg shadow p-6 flex flex-col items-center">
      <i class="fas fa-shield-alt fa-3x text-red-600 mb-4">
      </i>
      <h3 class="text-xl font-semibold mb-2">
       Safe &amp; Secure
      </h3>
      <p class="text-gray-700">
       Your personal and payment information is protected with us.
      </p>
     </div>
    </div>
   </div>
  </section>
  <!-- Footer -->
  <footer class="bg-gray-900 text-gray-300 py-12">
   <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 md:grid-cols-4 gap-8">
    <div>
     <h4 class="text-white font-bold text-lg mb-4">
      OYO
     </h4>
     <p class="text-gray-400 max-w-xs">
      OYO is your trusted partner for affordable and comfortable stays
          worldwide.
     </p>
     <div class="flex space-x-4 mt-4">
      <a aria-label="Facebook" class="hover:text-white" href="#">
       <i class="fab fa-facebook fa-lg">
       </i>
      </a>
      <a aria-label="Twitter" class="hover:text-white" href="#">
       <i class="fab fa-twitter fa-lg">
       </i>
      </a>
      <a aria-label="Instagram" class="hover:text-white" href="#">
       <i class="fab fa-instagram fa-lg">
       </i>
      </a>
      <a aria-label="LinkedIn" class="hover:text-white" href="#">
       <i class="fab fa-linkedin fa-lg">
       </i>
      </a>
     </div>
    </div>
    <div>
     <h4 class="text-white font-bold text-lg mb-4">
      Company
     </h4>
     <ul class="space-y-2">
      <li>
       <a class="hover:text-white" href="#">
        About Us
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Careers
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Blog
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Press
       </a>
      </li>
     </ul>
    </div>
    <div>
     <h4 class="text-white font-bold text-lg mb-4">
      Support
     </h4>
     <ul class="space-y-2">
      <li>
       <a class="hover:text-white" href="#">
        Help Center
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Cancellation Options
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Safety Information
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Contact Us
       </a>
      </li>
     </ul>
    </div>
    <div>
     <h4 class="text-white font-bold text-lg mb-4">
      Legal
     </h4>
     <ul class="space-y-2">
      <li>
       <a class="hover:text-white" href="#">
        Terms &amp; Conditions
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Privacy Policy
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Cookie Policy
       </a>
      </li>
      <li>
       <a class="hover:text-white" href="#">
        Security
       </a>
      </li>
     </ul>
    </div>
   </div>
   <div class="mt-12 text-center text-gray-500 text-sm">
    © 2024 OYO Clone. All rights reserved.
   </div>
  </footer>

  <!-- Login Modal -->
  <div aria-hidden="true" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 hidden" id="login-modal" role="dialog" aria-modal="true" aria-labelledby="login-modal-title">
   <div class="bg-white rounded-lg shadow-lg max-w-md w-full p-6 relative">
    <button aria-label="Close login modal" class="absolute top-3 right-3 text-gray-600 hover:text-gray-900 focus:outline-none" id="login-modal-close">
     <i class="fas fa-times fa-lg"></i>
    </button>
    <h3 class="text-2xl font-bold mb-4 text-center" id="login-modal-title">
     Login to OYO
    </h3>
    <form class="space-y-4" id="login-form">
     <div>
      <label class="block text-gray-700 font-semibold mb-1" for="login-email">
       Email
      </label>
      <input class="w-full border border-gray-300 rounded-md px-4 py-2 focus:outline-none focus:ring-2 focus:ring-red-600" id="login-email" name="email" placeholder="you@example.com" required="" type="email"/>
     </div>
     <div>
      <label class="block text-gray-700 font-semibold mb-1" for="login-password">
       Password
      </label>
      <input class="w-full border border-gray-300 rounded-md px-4 py-2 focus:outline-none focus:ring-2 focus:ring-red-600" id="login-password" name="password" placeholder="********" required="" type="password"/>
     </div>
     <button class="w-full bg-red-600 hover:bg-red-700 text-white font-semibold rounded-md px-4 py-2 transition" type="submit">
      Login
     </button>
    </form>
   </div>
  </div>

  <!-- Sign Up Modal -->
  <div aria-hidden="true" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50 hidden" id="signup-modal" role="dialog" aria-modal="true" aria-labelledby="signup-modal-title">
   <div class="bg-white rounded-lg shadow-lg max-w-md w-full p-6 relative">
    <button aria-label="Close sign up modal" class="absolute top-3 right-3 text-gray-600 hover:text-gray-900 focus:outline-none" id="signup-modal-close">
     <i class="fas fa-times fa-lg"></i>
    </button>
    <h3 class="text-2xl font-bold mb-4 text-center" id="signup-modal-title">
     Sign Up for OYO
    </h3>
    <form class="space-y-4" id="signup-form">
     <div>
      <label class="block text-gray-700 font-semibold mb-1" for="signup-name">
       Full Name
      </label>
      <input class="w-full border border-gray-300 rounded-md px-4 py-2 focus:outline-none focus:ring-2 focus:ring-red-600" id="signup-name" name="name" placeholder="Your full name" required="" type="text"/>
     </div>
     <div>
      <label class="block text-gray-700 font-semibold mb-1" for="signup-email">
       Email
      </label>
      <input class="w-full border border-gray-300 rounded-md px-4 py-2 focus:outline-none focus:ring-2 focus:ring-red-600" id="signup-email" name="email" placeholder="you@example.com" required="" type="email"/>
     </div>
     <div>
      <label class="block text-gray-700 font-semibold mb-1" for="signup-password">
       Password
      </label>
      <input class="w-full border border-gray-300 rounded-md px-4 py-2 focus:outline-none focus:ring-2 focus:ring-red-600" id="signup-password" name="password" placeholder="********" required="" type="password"/>
     </div>
     <button class="w-full bg-red-600 hover:bg-red-700 text-white font-semibold rounded-md px-4 py-2 transition" type="submit">
      Sign Up
     </button>
    </form>
   </div>
  </div>

  <script>
   // Mobile menu toggle
    const mobileMenuButton = document.getElementById('mobile-menu-button');
    const mobileMenu = document.getElementById('mobile-menu');

    mobileMenuButton.addEventListener('click', () => {
      mobileMenu.classList.toggle('hidden');
    });

    // Modal elements
    const loginButton = document.getElementById('login-button');
    const signupButton = document.getElementById('signup-button');
    const mobileLoginButton = document.getElementById('mobile-login-button');
    const mobileSignupButton = document.getElementById('mobile-signup-button');

    const loginModal = document.getElementById('login-modal');
    const signupModal = document.getElementById('signup-modal');

    const loginModalClose = document.getElementById('login-modal-close');
    const signupModalClose = document.getElementById('signup-modal-close');

    // Open modals
    loginButton.addEventListener('click', () => {
      loginModal.classList.remove('hidden');
    });
    signupButton.addEventListener('click', () => {
      signupModal.classList.remove('hidden');
    });
    mobileLoginButton.addEventListener('click', () => {
      loginModal.classList.remove('hidden');
      mobileMenu.classList.add('hidden');
    });
    mobileSignupButton.addEventListener('click', () => {
      signupModal.classList.remove('hidden');
      mobileMenu.classList.add('hidden');
    });

    // Close modals
    loginModalClose.addEventListener('click', () => {
      loginModal.classList.add('hidden');
    });
    signupModalClose.addEventListener('click', () => {
      signupModal.classList.add('hidden');
    });

    // Close modals on outside click
    window.addEventListener('click', (e) => {
      if (e.target === loginModal) {
        loginModal.classList.add('hidden');
      }
      if (e.target === signupModal) {
        signupModal.classList.add('hidden');
      }
    });

    // Optional: handle form submissions (just prevent default and close modal)
    document.getElementById('login-form').addEventListener('submit', (e) => {
      e.preventDefault();
      alert('Login form submitted!');
      loginModal.classList.add('hidden');
    });

    document.getElementById('signup-form').addEventListener('submit', (e) => {
      e.preventDefault();
      alert('Sign Up form submitted!');
      signupModal.classList.add('hidden');
    });
  </script>
 </body>
</html>
