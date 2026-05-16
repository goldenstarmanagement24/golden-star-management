export default function GoldenStarManagement() { return ( <div className="min-h-screen bg-black text-white font-sans"> {/* Hero Section */} <section className="relative overflow-hidden border-b border-yellow-600/30"> <div className="absolute inset-0 bg-gradient-to-br from-yellow-500/10 via-black to-black"></div>

<div className="relative z-10 max-w-7xl mx-auto px-6 py-24 grid lg:grid-cols-2 gap-12 items-center">
      <div>
        <div className="inline-flex items-center gap-2 border border-yellow-500/30 rounded-full px-4 py-2 text-sm text-yellow-400 mb-6">
          GOLDEN STAR MANAGEMENT
        </div>

        <h1 className="text-5xl md:text-7xl font-black leading-tight mb-6">
          Production
          <span className="block text-yellow-400">Audiovisuelle</span>
          & Management
        </h1>

        <p className="text-gray-300 text-lg leading-relaxed mb-8 max-w-xl">
          Une agence moderne spécialisée dans la production audiovisuelle,
          la gestion d’artistes, les événements, TikTok live, branding et
          création de contenu digital premium.
        </p>

        <div className="flex flex-wrap gap-4">
          <button className="bg-yellow-500 hover:bg-yellow-400 text-black font-bold px-8 py-4 rounded-2xl transition-all duration-300">
            Découvrir nos services
          </button>

          <button className="border border-yellow-500 text-yellow-400 hover:bg-yellow-500 hover:text-black font-bold px-8 py-4 rounded-2xl transition-all duration-300">
            Contact
          </button>
        </div>
      </div>

      <div className="flex justify-center">
        <div className="relative w-[380px] h-[380px] rounded-[40px] border border-yellow-500/30 bg-gradient-to-b from-yellow-500/20 to-black flex items-center justify-center shadow-2xl shadow-yellow-500/20 overflow-hidden">
          <img
            src="/mnt/data/1000024485.jpg"
            alt="Golden Star Management Logo"
            className="w-full h-full object-cover"
          />
        </div>
        </div>
      </div>
    </div>
  </section>

  {/* Services */}
  <section className="max-w-7xl mx-auto px-6 py-24">
    <div className="text-center mb-16">
      <h2 className="text-4xl md:text-5xl font-black mb-4 text-yellow-400">
        Nos Services
      </h2>
      <p className="text-gray-400 max-w-2xl mx-auto">
        Des solutions créatives haut de gamme pour les artistes, marques et créateurs de contenu.
      </p>
    </div>

    <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
      {[
        {
          title: 'Production Vidéo',
          desc: 'Clips, publicités, interviews et contenus premium.'
        },
        {
          title: 'Management',
          desc: 'Gestion d’artistes, influenceurs et talents digitaux.'
        },
        {
          title: 'TikTok Live',
          desc: 'Organisation de battles, événements et animations live.'
        },
        {
          title: 'Branding',
          desc: 'Création visuelle et identité digitale professionnelle.'
        }
      ].map((service, index) => (
        <div
          key={index}
          className="bg-zinc-900 border border-yellow-500/20 rounded-3xl p-8 hover:border-yellow-400 transition-all duration-300 hover:-translate-y-2"
        >
          <div className="w-14 h-14 rounded-2xl bg-yellow-500/10 border border-yellow-500/30 mb-6 flex items-center justify-center text-yellow-400 text-2xl font-bold">
            {index + 1}
          </div>

          <h3 className="text-2xl font-bold mb-4 text-yellow-300">
            {service.title}
          </h3>

          <p className="text-gray-400 leading-relaxed">
            {service.desc}
          </p>
        </div>
      ))}
    </div>
  </section>

  {/* Portfolio */}
  <section className="bg-zinc-950 border-y border-yellow-500/20 py-24 px-6">
    <div className="max-w-7xl mx-auto">
      <div className="flex flex-col md:flex-row md:items-end md:justify-between gap-6 mb-14">
        <div>
          <h2 className="text-4xl md:text-5xl font-black text-yellow-400 mb-4">
            Portfolio
          </h2>
          <p className="text-gray-400 max-w-2xl">
            Découvrez nos dernières productions et collaborations.
          </p>
        </div>

        <button className="border border-yellow-500 text-yellow-400 hover:bg-yellow-500 hover:text-black font-bold px-6 py-3 rounded-2xl transition-all duration-300">
          Voir tout
        </button>
      </div>

      <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
        {[1, 2, 3].map((item) => (
          <div
            key={item}
            className="h-[320px] rounded-3xl overflow-hidden relative border border-yellow-500/20 bg-gradient-to-b from-yellow-500/10 to-black group"
          >
            <div className="absolute inset-0 bg-black/40 group-hover:bg-black/20 transition-all duration-300"></div>

            <div className="absolute bottom-0 left-0 p-6 z-10">
              <div className="text-yellow-400 text-sm mb-2">
                PRODUCTION {item}
              </div>

              <h3 className="text-2xl font-bold">
                Projet Premium
              </h3>
            </div>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* Contact */}
  <section className="max-w-5xl mx-auto px-6 py-24 text-center">
    <h2 className="text-4xl md:text-6xl font-black mb-6 text-yellow-400">
      Ready To Shine?
    </h2>

    <p className="text-gray-400 text-lg max-w-2xl mx-auto mb-10 leading-relaxed">
      Contactez GOLDEN STAR MANAGEMENT pour développer votre image,
      produire votre contenu et faire évoluer votre marque.
    </p>

    <div className="flex flex-wrap justify-center gap-4">
      <button className="bg-yellow-500 hover:bg-yellow-400 text-black font-bold px-8 py-4 rounded-2xl transition-all duration-300">
        WhatsApp
      </button>

      <button className="border border-yellow-500 text-yellow-400 hover:bg-yellow-500 hover:text-black font-bold px-8 py-4 rounded-2xl transition-all duration-300">
        Instagram
      </button>
    </div>
  </section>

  {/* Footer */}
  <footer className="border-t border-yellow-500/20 py-8 px-6 text-center text-gray-500">
    © 2026 GOLDEN STAR MANAGEMENT — All Rights Reserved.
  </footer>
</div>

) }
