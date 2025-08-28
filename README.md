<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Llave Maestra 24/7 - Cerrajería</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100 font-sans">
  <!-- Encabezado -->
  <header class="bg-blue-900 text-white text-center p-6 shadow-lg">
    <h1 class="text-3xl font-bold">🔑 Llave Maestra 24/7</h1>
    <p class="text-lg">Cerrajería en Los Cabos - Servicio de Emergencia</p>
  </header>

  <!-- Servicios -->
  <section class="p-6 text-center">
    <h2 class="text-2xl font-semibold mb-4">Nuestros Servicios</h2>
    <div class="grid gap-6 md:grid-cols-3">
      <div class="bg-white rounded-2xl shadow-md p-4">
        <h3 class="font-bold text-xl mb-2">🚗 Apertura de coches</h3>
        <p>Abrimos vehículos de cualquier modelo, incluso polarizados.</p>
      </div>
      <div class="bg-white rounded-2xl shadow-md p-4">
        <h3 class="font-bold text-xl mb-2">🏠 Apertura de casas</h3>
        <p>Acceso rápido y seguro a tu hogar.</p>
      </div>
      <div class="bg-white rounded-2xl shadow-md p-4">
        <h3 class="font-bold text-xl mb-2">🔧 Cambio de chapas</h3>
        <p>Instalación y reemplazo de cerraduras para mayor seguridad.</p>
      </div>
    </div>
  </section>

  <!-- Botones de contacto -->
  <section class="p-6 text-center">
    <h2 class="text-2xl font-semibold mb-4">📞 Contáctanos</h2>
    <div class="flex flex-col md:flex-row justify-center gap-4">
      <!-- Botón de llamada de emergencia -->
      <a href="tel:+526711132883" class="bg-red-600 text-white px-6 py-3 rounded-2xl text-lg font-bold shadow-lg hover:bg-red-700">
        🚨 Llamada de Emergencia
      </a>

      <!-- Botón de WhatsApp con formulario automático -->
      <a id="whatsappBtn" target="_blank" class="bg-green-600 text-white px-6 py-3 rounded-2xl text-lg font-bold shadow-lg hover:bg-green-700">
        💬 Enviar WhatsApp
      </a>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-blue-900 text-white text-center p-4 mt-6">
    <p>&copy; 2025 Llave Maestra 24/7 | Los Cabos, BCS</p>
  </footer>

  <script>
    // Generar mensaje prellenado de WhatsApp con un pequeño "formulario"
    document.getElementById("whatsappBtn").addEventListener("click", function(){
      let nombre = prompt("Ingresa tu nombre:");
      let servicio = prompt("¿Qué servicio necesitas? (coche / casa / chapa)");
      let detalles = prompt("Escribe detalles: modelo de coche, si tiene polarizado o adjunta foto de la chapa");

      let mensaje = `Hola, soy ${nombre}. Necesito servicio de ${servicio}. Detalles: ${detalles}`;

      let url = `https://wa.me/526711132883?text=${encodeURIComponent(mensaje)}`;
      window.open(url, "_blank");
    });
  </script>
</body>
</html>
