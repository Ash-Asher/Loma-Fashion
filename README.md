export default function LomaFashionWebsite() {
  return (
    <div className="min-h-screen bg-neutral-950 text-white font-sans">
      {/* Hero Section */}
      <section className="relative overflow-hidden">
        <div className="absolute inset-0 bg-gradient-to-br from-pink-500/20 via-transparent to-orange-500/20 blur-3xl" />

        <div className="relative max-w-7xl mx-auto px-6 py-24 lg:py-36 grid lg:grid-cols-2 gap-14 items-center">
          <div>
            <span className="inline-block px-4 py-2 rounded-full bg-white/10 border border-white/10 text-sm tracking-wide uppercase">
              Loma Fashion
            </span>

            <h1 className="mt-6 text-5xl lg:text-7xl font-black leading-tight">
              Neue Trends,
              <br />
              Neuer Style.
            </h1>

            <p className="mt-6 text-lg text-neutral-300 leading-relaxed max-w-xl">
              Jeder Look ein neues Teil. Entdecke moderne Streetwear,
              elegante Outfits und angesagte Fashion-Pieces für deinen
              individuellen Style.
            </p>

            <div className="mt-10 flex flex-wrap gap-4">
              <button className="px-7 py-4 rounded-2xl bg-white text-black font-semibold hover:scale-105 transition-transform shadow-2xl">
                Jetzt shoppen
              </button>

              <button className="px-7 py-4 rounded-2xl border border-white/20 hover:bg-white/10 transition">
                Neue Kollektion
              </button>
            </div>
          </div>

          <div className="relative">
            <div className="absolute -top-10 -left-10 w-48 h-48 bg-pink-500 rounded-full blur-3xl opacity-30" />
            <div className="absolute bottom-0 right-0 w-56 h-56 bg-orange-500 rounded-full blur-3xl opacity-20" />

            <div className="relative grid grid-cols-2 gap-5">
              <img
                src="https://images.unsplash.com/photo-1529139574466-a303027c1d8b?q=80&w=1200&auto=format&fit=crop"
                alt="Fashion Model"
                className="rounded-3xl h-[420px] object-cover shadow-2xl"
              />

              <div className="space-y-5 mt-10">
                <img
                  src="https://images.unsplash.com/photo-1496747611176-843222e1e57c?q=80&w=1200&auto=format&fit=crop"
                  alt="Fashion Style"
                  className="rounded-3xl h-[200px] w-full object-cover shadow-2xl"
                />

                <img
                  src="https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?q=80&w=1200&auto=format&fit=crop"
                  alt="Modern Outfit"
                  className="rounded-3xl h-[200px] w-full object-cover shadow-2xl"
                />
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Collection Section */}
      <section className="max-w-7xl mx-auto px-6 py-20">
        <div className="flex items-end justify-between flex-wrap gap-6 mb-12">
          <div>
            <p className="text-pink-400 uppercase tracking-[0.3em] text-sm">
              Neue Kollektion
            </p>
            <h2 className="text-4xl lg:text-5xl font-bold mt-3">
              Fashion Highlights
            </h2>
          </div>

          <p className="text-neutral-400 max-w-lg">
            Von minimalistischen Essentials bis zu auffälligen Trend-Pieces –
            finde Outfits, die deinen Look auf das nächste Level bringen.
          </p>
        </div>

        <div className="grid md:grid-cols-3 gap-8">
          {[
            {
              title: 'Urban Streetwear',
              image:
                'https://images.unsplash.com/photo-1483985988355-763728e1935b?q=80&w=1200&auto=format&fit=crop',
            },
            {
              title: 'Modern Elegance',
              image:
                'https://images.unsplash.com/photo-1521572267360-ee0c2909d518?q=80&w=1200&auto=format&fit=crop',
            },
            {
              title: 'Summer Vibes',
              image:
                'https://images.unsplash.com/photo-1503342217505-b0a15ec3261c?q=80&w=1200&auto=format&fit=crop',
            },
          ].map((item) => (
            <div
              key={item.title}
              className="group bg-white/5 border border-white/10 rounded-3xl overflow-hidden hover:-translate-y-2 transition duration-300 shadow-xl"
            >
              <div className="overflow-hidden">
                <img
                  src={item.image}
                  alt={item.title}
                  className="h-80 w-full object-cover group-hover:scale-105 transition duration-500"
                />
              </div>

              <div className="p-6">
                <h3 className="text-2xl font-semibold">{item.title}</h3>
                <p className="mt-3 text-neutral-400">
                  Stylische Outfits mit modernen Designs und hochwertigen
                  Materialien.
                </p>
              </div>
            </div>
          ))}
        </div>
      </section>

      {/* About Section */}
      <section className="bg-white text-black py-24">
        <div className="max-w-6xl mx-auto px-6 grid lg:grid-cols-2 gap-14 items-center">
          <img
            src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?q=80&w=1200&auto=format&fit=crop"
            alt="Loma Fashion Store"
            className="rounded-3xl shadow-2xl h-[500px] w-full object-cover"
          />

          <div>
            <p className="uppercase tracking-[0.3em] text-sm text-neutral-500">
              Über Uns
            </p>

            <h2 className="text-4xl lg:text-5xl font-bold mt-4 leading-tight">
              Fashion bedeutet Persönlichkeit.
            </h2>

            <p className="mt-6 text-lg text-neutral-700 leading-relaxed">
              Loma Fashion steht für moderne Styles, mutige Kombinationen und
              individuelle Looks. Unsere Mission ist es, dir jeden Tag neue
              Inspiration für dein perfektes Outfit zu geben.
            </p>

            <div className="mt-10 grid grid-cols-2 gap-6">
              <div className="p-6 rounded-2xl bg-neutral-100">
                <h3 className="text-3xl font-black">500+</h3>
                <p className="mt-2 text-neutral-600">Neue Fashion-Pieces</p>
              </div>

              <div className="p-6 rounded-2xl bg-neutral-100">
                <h3 className="text-3xl font-black">24/7</h3>
                <p className="mt-2 text-neutral-600">Online verfügbar</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Newsletter */}
      <section className="max-w-5xl mx-auto px-6 py-24">
        <div className="rounded-[2rem] bg-gradient-to-r from-pink-500 to-orange-500 p-10 lg:p-16 text-center shadow-2xl">
          <h2 className="text-4xl lg:text-5xl font-black">
            Bleibe im Trend
          </h2>

          <p className="mt-5 text-lg text-white/90 max-w-2xl mx-auto">
            Erhalte exklusive Angebote, neue Kollektionen und die neuesten
            Fashion-News direkt in dein Postfach.
          </p>

          <div className="mt-10 flex flex-col sm:flex-row gap-4 justify-center">
            <input
              type="email"
              placeholder="Deine E-Mail"
              className="px-6 py-4 rounded-2xl w-full sm:w-96 text-black outline-none"
            />

            <button className="px-8 py-4 rounded-2xl bg-black text-white font-semibold hover:scale-105 transition-transform">
              Abonnieren
            </button>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t border-white/10 py-10 px-6">
        <div className="max-w-7xl mx-auto flex flex-col md:flex-row justify-between gap-6 items-center">
          <div>
            <h3 className="text-2xl font-black">Loma Fashion</h3>
            <p className="text-neutral-400 mt-2">
              Neue Trends, Neuer Style, jeder Look ein neues Teil.
            </p>
          </div>

          <div className="flex gap-6 text-neutral-400">
            <a href="#" className="hover:text-white transition">
              Instagram
            </a>
            <a href="#" className="hover:text-white transition">
              TikTok
            </a>
            <div className="text-neutral-400 hover:text-white transition">
              Kontakt: 01731234567
            </div>
          </div>
        </div>
      </footer>
    </div>
  )
}
