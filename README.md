# Car-website
Day1week2 (w2) ( Wach in raw)


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Auth Page</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    body {
      background-image: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTLgppPJBTR9z6puEwJc7VXc7fYezLtpvTIBg&s');
      background-size: cover;
      background-position: center;
      font-family: sans-serif;
    }
  </style>
</head>
<body class="bg-black bg-opacity-60 text-white min-h-screen flex items-center justify-center">

  <!-- Main auth selection -->
  <div id="main" class="space-y-6 text-center">
    <h1 class="text-3xl font-bold">Welcome</h1>
    <div class="space-x-4">
      <button onclick="showLogin()" class="bg-blue-600 hover:bg-blue-700 px-6 py-2 rounded">Log In</button>
      <button onclick="showSignup()" class="bg-green-600 hover:bg-green-700 px-6 py-2 rounded">Sign Up</button>
    </div>
  </div>

  <!-- Login Form -->
  <div id="login" class="hidden bg-white bg-opacity-90 text-black p-6 rounded-xl shadow-md w-full max-w-sm">
    <a href="#" onclick="goBack()" class="text-blue-600 font-semibold">&larr; Go back to main page</a>
    <h2 class="text-2xl font-bold text-center my-4">Log In</h2>
    <form onsubmit="handleSubmit(event)">
      <input type="email" placeholder="Email" required class="w-full p-2 mb-4 border rounded" />
      <input type="password" placeholder="Password" required class="w-full p-2 mb-4 border rounded" />
      <button type="submit" class="w-full bg-blue-600 text-white py-2 rounded hover:bg-blue-700">Log In</button>
    </form>
  </div>

  <!-- Signup Form -->
  <div id="signup" class="hidden bg-white bg-opacity-90 text-black p-6 rounded-xl shadow-md w-full max-w-sm">
    <a href="#" onclick="goBack()" class="text-blue-600 font-semibold">&larr; Go back to main page</a>
    <h2 class="text-2xl font-bold text-center my-4">Sign Up</h2>
    <form onsubmit="handleSubmit(event)">
      <input type="text" placeholder="First Name" required class="w-full p-2 mb-3 border rounded" />
      <input type="text" placeholder="Last Name" required class="w-full p-2 mb-3 border rounded" />
      <input type="email" placeholder="Email" required class="w-full p-2 mb-3 border rounded" />
      <input type="password" placeholder="Password" required class="w-full p-2 mb-3 border rounded" />
      <div class="flex gap-2 mb-3">
        <select class="p-2 border rounded bg-white">
          <option value="+1">+1</option>
          <option value="+44">+44</option>
          <option value="+373" selected>+373</option>
          <option value="+91">+91</option>
        </select>
        <input type="tel" placeholder="Phone" required class="flex-1 p-2 border rounded" />
      </div>
      <button type="submit" class="w-full bg-green-600 text-white py-2 rounded hover:bg-green-700">Sign Up</button>
    </form>
  </div>

  <!-- Car Gallery Page -->
  <div id="gallery" class="hidden bg-black bg-opacity-70 text-white min-h-screen p-6">
    <a href="#" onclick="logOut()" class="text-white bg-red-600 hover:bg-red-700 px-4 py-2 rounded fixed top-4 left-4">Log Out</a>

    <h1 class="text-3xl font-bold text-center mb-8">🚗 Luxury Car Gallery 🚗</h1>

    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxW_Ima2UvWlCRCT1n1jCFdhRat-s8sUK7pQ&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcReH9fJERh9aU7OsmC3KYu40Ifs-dlRw962_A&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTeoDx9gkbVVGlaaqO33ybkNLzftacoYxv0WQ&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSWtyoKr8-EgU3I8xH4GlEJiPOqPszxHJLWcw&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSrQY9RaGIGtMbJE1VePWT9v5h1pDGySLvAnA&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQdIIeYSZK0HDOoK_zkubYuaXMwB0NQx7JITQ&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRISqfw-DyZmmwLex-xhVmKuzlOWR5jOi7VnA&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQmk_lgQUqT5D75lNP_fj24ToEUCNCA-_iCJg&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT7UYUrcJi_OK_u4Q-xLgEs9E9V88ZbzKSXCg&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRNAJdBeuqRpLoNNITBW-9vdIOV3uqbQVoq3Q&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTkVUlCFjrcAd8KtMXDNmqP4SA_nhCTINkwow&s" class="rounded-xl shadow-lg" />
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9u-C4KJbMEnHI1yYgnzz1wua0mhVr6S3DGA&s" class="rounded-xl shadow-lg" />
    </div>
  </div>

  <script>
    function showLogin() {
      document.getElementById('main').style.display = 'none';
      document.getElementById('login').style.display = 'block';
    }

    function showSignup() {
      document.getElementById('main').style.display = 'none';
      document.getElementById('signup').style.display = 'block';
    }

    function goBack() {
      document.getElementById('login').style.display = 'none';
      document.getElementById('signup').style.display = 'none';
      document.getElementById('main').style.display = 'block';
    }

    function handleSubmit(event) {
      event.preventDefault();

      const form = event.target;
      const email = form.querySelector('input[type="email"]')?.value.trim();
      const password = form.querySelector('input[type="password"]')?.value;
      const phoneInput = form.querySelector('input[type="tel"]');
      const phone = phoneInput ? phoneInput.value.trim() : null;

      if (!email.endsWith('@gmail.com')) {
        alert('Email-ul trebuie să fie de tip @gmail.com');
        return;
      }

      if (password.length < 8) {
        alert('Parola trebuie să conțină minim 8 caractere.');
        return;
      }

      if (phoneInput && !/^\d{8}$/.test(phone)) {
        alert('Numărul de telefon trebuie să conțină exact 8 cifre.');
        return;
      }

      document.getElementById('main').style.display = 'none';
      document.getElementById('login').style.display = 'none';
      document.getElementById('signup').style.display = 'none';
      document.getElementById('gallery').style.display = 'block';
    }

    function logOut() {
      document.getElementById('gallery').style.display = 'none';
      document.getElementById('main').style.display = 'block';
    }
  </script>
</body>
</html>
