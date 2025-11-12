"use client";

import Image from "next/image";

export default function Home() {
  // WhatsApp contacto Pedro
  const whatsappNumber = "573102668311";
  const whatsappMessage = encodeURIComponent(
    "Hola, quisiera información sobre el arriendo de parqueadero en la Calle 162 con Cra 54"
  );
  const whatsappLink = `https://wa.me/${whatsappNumber}?text=${whatsappMessage}`;

  return (
    <main className="min-h-screen bg-white text-slate-900">
      <section className="max-w-2xl mx-auto px-4 py-12 flex flex-col items-center space-y-8">
        <h1 className="text-3xl md:text-5xl font-bold text-center">
          ARRIENDO PARQUEDERO Calle 162 con Cra 54 CONJUNTO CERRADO
        </h1>

        <div className="flex flex-col md:flex-row gap-4 w-full justify-center">
          <Image
            alt="Parqueadero cerrado"
            src="/2025-04-04-02-37-33.jpg"
            className="rounded-xl shadow-lg"
            width={470}
            height={360}
            priority
          />
          <Image
            alt="Conjunto cerrado -- sirve para cualquier automóvil"
            src="/PARQUEADERO-ALQUILER-COLINA-CAMPESTRE-MAZUREN-BRISS-DE-SOTAVENTO-AUTONORTE.jpg"
            className="rounded-xl shadow-lg"
            width={470}
            height={360}
            priority
          />
        </div>

        <h2 className="mt-6 text-xl md:text-2xl text-center font-semibold">
          DISPONIBLE - ARRIENDO PARQUEDERO MAZUREN – CANTALEJO – ALEJANDRÍA – GILMAR – DE MUY FACIL PARQUEO en la Calle 162 con Cra 54 para cualquier tipo de automóvil AL LADO DEL CARMEL CLUB - En conjunto cerrado residencial con seguridad las 24 horas.
          <br /><br />
          WhatsApp Pedro +57 310 266 83 11 o Llamar SONIA 313 479 81 50
        </h2>

        <a href={whatsappLink} target="_blank" rel="noopener noreferrer">
          <button className="bg-green-600 text-white text-xl font-bold px-7 py-5 rounded-full shadow-xl hover:bg-green-700 transition">
            INFORMES por WhatsApp
          </button>
        </a>

        <div className="w-full mt-10" style={{ minHeight: 380 }}>
          <iframe
            src="https://maps.app.goo.gl/e5cA2DGMbuXypALp6"
            width="100%"
            height="380"
            style={{ border: 0 }}
            allowFullScreen=""
            loading="lazy"
            referrerPolicy="no-referrer-when-downgrade"
            title="Mapa Parqueadero Calle 162"
          ></iframe>
        </div>
      </section>
    </main>
  );
}
