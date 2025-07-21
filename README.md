# Bmw-m3-e46.
Все о легенде 
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>BMW M3 E46 | Легенда скорости</title>
  <script src="http://cdn.tailwindcss.com"></script>
  <style>
    body {
      background-color: #0d0d0d;
      color: white;
    }
  </style>
</head>
<body class="font-sans">

  <!-- Шапка -->
  <header class="bg-black text-white py-6 shadow-lg">
    <div class="container mx-auto px-4 text-center">
      <h1 class="text-4xl font-bold text-red-600 uppercase">BMW M3 E46</h1>
      <p class="text-gray-400 text-sm sm:text-base mt-2">Легенда среди M-серии. Гоночная душа.</p>
    </div>
  </header>

  <!-- Обзор -->
  <section class="py-10 px-4 max-w-3xl mx-auto">
    <h2 class="text-2xl font-semibold text-red-500 mb-4">Обзор</h2>
    <p class="text-gray-300 leading-relaxed">
      BMW M3 E46 — это сочетание точной управляемости, мощного атмосферного двигателя и классического дизайна начала 2000-х.
      Оснащён рядной шестёркой S54 с 343 л.с., задним приводом и механикой — этот автомобиль стал иконой эпохи.
    </p>
    <img src="https://cdn.pixabay.com/photo/2017/03/27/13/37/bmw-2174018_1280.jpg" 
         alt="BMW M3 E46" 
         class="rounded-xl shadow-xl mt-6 w-full h-auto">
  </section>

  <!-- Галерея -->
  <section class="py-10 px-4 max-w-4xl mx-auto">
    <h2 class="text-2xl font-semibold text-red-500 mb-4 text-center">Галерея</h2>
    <div class="relative">
      <img id="galleryImage" src="https://cdn.pixabay.com/photo/2020/01/01/20/33/bmw-4735000_1280.jpg" 
           alt="Галерея" 
           class="rounded-xl shadow-lg w-full h-auto">
      <div class="flex justify-between mt-4">
        <button onclick="prevImage()" class="bg-red-600 px-4 py-2 rounded text-sm">Назад</button>
        <button onclick="nextImage()" class="bg-red-600 px-4 py-2 rounded text-sm">Вперёд</button>
      </div>
    </div>
  </section>

  <script>
    const images = [
      "https://cdn.pixabay.com/photo/2020/01/01/20/33/bmw-4735000_1280.jpg",
      "https://cdn.pixabay.com/photo/2022/10/28/13/44/bmw-7552254_1280.jpg",
      "https://cdn.pixabay.com/photo/2018/06/08/16/56/bmw-3465205_1280.jpg"
    ];
    let current = 0;
    const galleryImage = document.getElementById("galleryImage");
    function nextImage() {
      current = (current + 1) % images.length;
      galleryImage.src = images[current];
    }
    function prevImage() {
      current = (current - 1 + images.length) % images.length;
      galleryImage.src = images[current];
    }
  </script>

  <!-- Видеообзор -->
  <section class="py-10 px-4 max-w-4xl mx-auto">
    <h2 class="text-2xl font-semibold text-red-500 mb-4 text-center">Видеообзор</h2>
    <div class="aspect-w-16 aspect-h-9">
      <iframe class="w-full rounded-xl shadow-lg" height="315"
        src="https://www.youtube.com/embed/jRCE4Zw4O2Y" 
        title="BMW M3 E46 Review" 
        frameborder="0" allowfullscreen></iframe>
    </div>
  </section>

  <!-- Интересные факты -->
  <section class="py-10 px-4 max-w-3xl mx-auto">
    <h2 class="text-2xl font-semibold text-red-500 mb-4">Интересные факты</h2>
    <ul class="text-gray-300 list-disc pl-5 space-y-2">
      <li>Красная зона тахометра повышается по мере прогрева двигателя.</li>
      <li>Уникальный двигатель S54 признан одним из лучших атмосферников BMW.</li>
      <li>Выпускалась с 2000 по 2006 год, в кузовах купе, кабриолет и редкий седан.</li>
      <li>Имеет отдельные версии CSL (ещё легче и злее).</li>
    </ul>
  </section>

  <!-- Сравнение -->
  <section class="py-10 px-4 max-w-4xl mx-auto">
    <h2 class="text-2xl font-semibold text-red-500 mb-4 text-center">Сравнение с другими M3</h2>
    <div class="overflow-x-auto">
      <table class="min-w-full text-left text-gray-300 border border-gray-700">
        <thead class="bg-red-800 text-white">
          <tr>
            <th class="py-2 px-4 border border-gray-700">Модель</th>
            <th class="py-2 px-4 border border-gray-700">Мощность</th>
            <th class="py-2 px-4 border border-gray-700">0-100 км/ч</th>
            <th class="py-2 px-4 border border-gray-700">Двигатель</th>
          </tr>
        </thead>
        <tbody>
          <tr class="bg-gray-900">
            <td class="py-2 px-4 border border-gray-700">M3 E36</td>
            <td class="py-2 px-4 border border-gray-700">286-321 л.с.</td>
            <td class="py-2 px-4 border border-gray-700">5.5–5.2 сек</td>
            <td class="py-2 px-4 border border-gray-700">Р6 (S50)</td>
          </tr>
          <tr class="bg-gray-800">
            <td class="py-2 px-4 border border-gray-700">M3 E46</td>
            <td class="py-2 px-4 border border-gray-700">343 л.с.</td>
            <td class="py-2 px-4 border border-gray-700">5.1 сек</td>
            <td class="py-2 px-4 border border-gray-700">Р6 (S54)</td>
          </tr>
          <tr class="bg-gray-900">
            <td class="py-2 px-4 border border-gray-700">M3 E92</td>
            <td class="py-2 px-4 border border-gray-700">420 л.с.</td>
            <td class="py-2 px-4 border border-gray-700">4.8 сек</td>
            <td class="py-2 px-4 border border-gray-700">V8 (S65)</td>
          </tr>
        </tbody>
      </table>
    </div>
  </section>

  <!-- Комментарии -->
  <section class="py-10 px-4 max-w-4xl mx-auto">
    <h2 class="text-2xl font-semibold text-red-500 mb-4 text-center">Комментарии</h2>
    <div id="disqus_thread"></div>
    <script>
      var disqus_config = function () {
        this.page.url = window.location.href;
        this.page.identifier = "bmw-m3-e46-site";
      };
      (function() {
        var d = document, s = d.createElement('script');
        s.src = 'http://EXAMPLE.disqus.com/embed.js';  // ← ЗАМЕНИ "EXAMPLE" на свой Disqus shortname
        s.setAttribute('data-timestamp', +new Date());
        (d.head || d.body).appendChild(s);
      })();
    </script>
  </section>

  <!-- Футер -->
  <footer class="bg-black text-center text-gray-500 text-sm py-6 mt-10">
    © 2025 BMW M3 E46 Fan Site. Создано для ценителей скорости.
  </footer>

</body>
</html>
