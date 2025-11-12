"use client";

export default function Home() {
  const whatsappNumber = "573102668311";
  const whatsappMessage = encodeURIComponent(
    "Hola, quisiera información sobre el arriendo de parqueadero en la Calle 162 con Cra 54"
  );
  const whatsappLink = `https://wa.me/${whatsappNumber}?text=${whatsappMessage}`;

  return (
    <main className="min-h-screen bg-white text-slate-900">
      <section className="max-w-2xl mx-auto px-4 py-12 flex flex-col items-center space-y-8">
        <h1 className="text-3xl md:text-5xl font-bold text-center">
          ARRIENDO PARQUEADERO Calle 162 con Cra 54 - CONJUNTO CERRADO
        </h1>

        <div className="flex flex-col md:flex-row gap-4 w-full justify-center">
          <img
            alt="Entrada del parqueadero en conjunto cerrado"
            src="/2025-04-04-02-37-33.jpg"
            className="rounded-xl shadow-lg"
            width={470}
            height={360}
            loading="lazy"
            style={{ objectFit: "cover" }}
          />
          <img
            alt="Plaza de parqueo, apta para cualquier automóvil"
            src="/PARQUEADERO-ALQUILER-COLINA-CAMPESTRE-MAZUREN-BRISS-DE-SOTAVENTO-AUTONORTE.jpg"
            className="rounded-xl shadow-lg"
            width={470}
            height={360}
            loading="lazy"
            style={{ objectFit: "cover" }}
          />
        </div>

        <h2 className="mt-6 text-xl md:text-2xl text-center font-semibold">
          DISPONIBLE - ARRIENDO PARQUEADERO MAZUREN – CANTALEJO – ALEJANDRÍA – GILMAR – DE MUY FÁCIL PARQUEO en la Calle 162 con Cra 54 para cualquier tipo de automóvil. AL LADO DEL CARMEL CLUB - En conjunto cerrado residencial con seguridad las 24 horas.
          <br />
          <br />
          WhatsApp:{" "}
          <a
            href={whatsappLink}
            target="_blank"
            rel="noopener noreferrer"
            aria-label="Enviar mensaje por WhatsApp a Pedro"
            className="text-green-600 font-bold underline"
          >
            Pedro +57 310 266 83 11
          </a>{" "}
          o llamar:{" "}
          <a href="tel:+573134798150" className="text-blue-600 font-semibold underline">
            Sonia 313 479 81 50
          </a>
        </h2>

        <a
          href={whatsappLink}
          target="_blank"
          rel="noopener noreferrer"
          aria-label="Enviar mensaje por WhatsApp a Pedro"
          className="bg-green-600 text-white text-xl font-bold px-7 py-5 rounded-full shadow-xl hover:bg-green-700 transition"
        >
          INFORMES por WhatsApp
        </a>

        <div className="w-full mt-10" style={{ minHeight: 380 }}>
          <iframe
            src="https://maps.app.goo.gl/e5cA2DGMbuXypALp6"
            width="100%"
            height="380"
            style={{ border: 0 }}
            allowFullScreen
            loading="lazy"
            referrerPolicy="no-referrer-when-downgrade"
            title="Mapa Parqueadero Calle 162"
          />
        </div>
      </section>
    </main>
  );
}
