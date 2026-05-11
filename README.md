export default function PSLGolfWebsite() {
  return (
    <div className="min-h-screen bg-zinc-950 text-white font-sans">
      {/* Header */}
      <header className="sticky top-0 z-50 bg-black/80 backdrop-blur border-b border-zinc-800">
        <div className="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
          <div>
            <h1 className="text-2xl font-bold tracking-wide">PSL Mobile Golf Simulator</h1>
            <p className="text-sm text-zinc-400">Premier Swing Lounge Delivered To You</p>
          </div>

          <nav className="hidden md:flex gap-8 text-sm font-medium">
            <a href="#home" className="hover:text-green-400 transition">Home</a>
            <a href="#services" className="hover:text-green-400 transition">Services</a>
            <a href="#contact" className="hover:text-green-400 transition">Contact</a>
          </nav>

          <a
            href="#contact"
            className="bg-green-500 hover:bg-green-400 text-black font-semibold px-5 py-3 rounded-2xl transition shadow-lg"
          >
            Book Your Event
          </a>
        </div>
      </header>

      {/* Hero Section */}
      <section
        id="home"
        className="relative overflow-hidden"
      >
        <div className="absolute inset-0 bg-[url('https://images.unsplash.com/photo-1535131749006-b7f58c99034b?q=80&w=2070&auto=format&fit=crop')] bg-cover bg-center opacity-30"></div>

        <div className="relative max-w-7xl mx-auto px-6 py-32 grid lg:grid-cols-2 gap-16 items-center">
          <div>
            <div className="inline-flex items-center gap-2 bg-zinc-900/70 border border-zinc-700 rounded-full px-4 py-2 mb-6">
              <span className="w-2 h-2 bg-green-400 rounded-full"></span>
              <p className="text-sm text-zinc-300">Serving Events Across Central Florida</p>
            </div>

            <h2 className="text-5xl md:text-7xl font-black leading-tight mb-6">
              Bring The <span className="text-green-400">Golf Experience</span> Anywhere
            </h2>

            <p className="text-lg text-zinc-300 mb-8 max-w-xl leading-relaxed">
              PSL Mobile Golf Simulator brings premium virtual golf entertainment directly to your home, corporate event, birthday party, tournament, or private gathering.
            </p>

            <div className="flex flex-wrap gap-4">
              <a
                href="#contact"
                className="bg-green-500 hover:bg-green-400 text-black font-bold px-8 py-4 rounded-2xl transition shadow-xl"
              >
                Book Your Event
              </a>

              <a
                href="#services"
                className="border border-zinc-600 hover:border-green-400 hover:text-green-400 px-8 py-4 rounded-2xl transition"
              >
                View Services
              </a>
            </div>
          </div>

          <div className="grid grid-cols-2 gap-4">
            <div className="bg-zinc-900/70 border border-zinc-800 rounded-3xl p-8 backdrop-blur">
              <h3 className="text-4xl font-black text-green-400 mb-2">100+</h3>
              <p className="text-zinc-300">Virtual Golf Courses</p>
            </div>

            <div className="bg-zinc-900/70 border border-zinc-800 rounded-3xl p-8 backdrop-blur mt-12">
              <h3 className="text-4xl font-black text-green-400 mb-2">4K</h3>
              <p className="text-zinc-300">Immersive Simulator Display</p>
            </div>

            <div className="bg-zinc-900/70 border border-zinc-800 rounded-3xl p-8 backdrop-blur -mt-6">
              <h3 className="text-4xl font-black text-green-400 mb-2">Indoor</h3>
              <p className="text-zinc-300">Weather-Proof Entertainment</p>
            </div>

            <div className="bg-zinc-900/70 border border-zinc-800 rounded-3xl p-8 backdrop-blur mt-6">
              <h3 className="text-4xl font-black text-green-400 mb-2">Events</h3>
              <p className="text-zinc-300">Perfect For Any Occasion</p>
            </div>
          </div>
        </div>
      </section>

      {/* Services Section */}
      <section id="services" className="py-24 bg-zinc-900">
        <div className="max-w-7xl mx-auto px-6">
          <div className="text-center mb-16">
            <p className="text-green-400 font-semibold tracking-widest uppercase mb-4">
              Our Services
            </p>

            <h2 className="text-5xl font-black mb-6">
              Golf Entertainment For Every Event
            </h2>

            <p className="text-zinc-400 max-w-3xl mx-auto text-lg">
              From backyard parties to large corporate activations, PSL Mobile Golf Simulator delivers a premium golf experience anywhere you need it.
            </p>
          </div>

          <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
            {[
              {
                title: 'Corporate Events',
                desc: 'Boost engagement at company parties, networking events, conferences, and team-building experiences.',
              },
              {
                title: 'Birthday Parties',
                desc: 'Create a fun and unforgettable golf experience for adults, teens, and kids.',
              },
              {
                title: 'Weddings & Private Events',
                desc: 'Add unique entertainment guests will remember with interactive golf competitions and games.',
              },
              {
                title: 'Golf Tournaments',
                desc: 'Enhance tournament experiences with closest-to-the-pin contests, warmups, and sponsor activations.',
              },
              {
                title: 'Community Events',
                desc: 'Perfect for schools, churches, festivals, HOA gatherings, and neighborhood events.',
              },
              {
                title: 'Training & Practice',
                desc: 'Use advanced simulator data and virtual courses to sharpen your golf game year-round.',
              },
            ].map((service, index) => (
              <div
                key={index}
                className="bg-black border border-zinc-800 rounded-3xl p-8 hover:border-green-400 transition duration-300 hover:-translate-y-2"
              >
                <div className="w-14 h-14 bg-green-500/10 border border-green-500/30 rounded-2xl flex items-center justify-center mb-6">
                  <span className="text-2xl">⛳</span>
                </div>

                <h3 className="text-2xl font-bold mb-4">{service.title}</h3>
                <p className="text-zinc-400 leading-relaxed">{service.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* CTA Banner */}
      <section className="py-20 px-6">
        <div className="max-w-6xl mx-auto bg-gradient-to-r from-green-500 to-green-300 rounded-[32px] p-12 text-black text-center shadow-2xl">
          <h2 className="text-4xl md:text-5xl font-black mb-6">
            Ready To Elevate Your Next Event?
          </h2>

          <p className="text-lg mb-8 max-w-3xl mx-auto font-medium">
            Book PSL Mobile Golf Simulator today and bring a premium golf entertainment experience directly to your guests.
          </p>

          <a
            href="#contact"
            className="inline-block bg-black text-white hover:bg-zinc-900 px-8 py-4 rounded-2xl font-bold transition"
          >
            Book Your Event
          </a>
        </div>
      </section>

      {/* Contact Section */}
      <section id="contact" className="py-24 bg-black">
        <div className="max-w-7xl mx-auto px-6 grid lg:grid-cols-2 gap-16 items-start">
          <div>
            <p className="text-green-400 font-semibold tracking-widest uppercase mb-4">
              Contact Us
            </p>

            <h2 className="text-5xl font-black mb-6">
              Let’s Plan Your Event
            </h2>

            <p className="text-zinc-400 text-lg leading-relaxed mb-10 max-w-xl">
              Tell us about your event, preferred date, and guest count. We’ll help customize the perfect mobile golf simulator experience for your occasion.
            </p>

            <div className="space-y-6 text-zinc-300">
              <div className="flex items-center gap-4">
                <div className="w-12 h-12 rounded-2xl bg-zinc-900 flex items-center justify-center border border-zinc-800">
                  📍
                </div>
                <div>
                  <p className="font-semibold">Service Area</p>
                  <p className="text-zinc-500">Central Florida & Surrounding Areas</p>
                </div>
              </div>

              <div className="flex items-center gap-4">
                <div className="w-12 h-12 rounded-2xl bg-zinc-900 flex items-center justify-center border border-zinc-800">
                  📞
                </div>
                <div>
                  <p className="font-semibold">Phone</p>
                  <p className="text-zinc-500">(407) 555-1234</p>
                </div>
              </div>

              <div className="flex items-center gap-4">
                <div className="w-12 h-12 rounded-2xl bg-zinc-900 flex items-center justify-center border border-zinc-800">
                  ✉️
                </div>
                <div>
                  <p className="font-semibold">Email</p>
                  <p className="text-zinc-500">bookings@pslgolf.com</p>
                </div>
              </div>
            </div>
          </div>

          <div className="bg-zinc-900 border border-zinc-800 rounded-[32px] p-10 shadow-2xl">
            <form className="space-y-6">
              <div>
                <label className="block text-sm font-medium mb-2">Full Name</label>
                <input
                  type="text"
                  placeholder="Enter your name"
                  className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-green-400"
                />
              </div>

              <div>
                <label className="block text-sm font-medium mb-2">Email Address</label>
                <input
                  type="email"
                  placeholder="Enter your email"
                  className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-green-400"
                />
              </div>

              <div>
                <label className="block text-sm font-medium mb-2">Phone Number</label>
                <input
                  type="tel"
                  placeholder="Enter your phone number"
                  className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-green-400"
                />
              </div>

              <div>
                <label className="block text-sm font-medium mb-2">Event Type</label>
                <select className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-green-400">
                  <option>Corporate Event</option>
                  <option>Birthday Party</option>
                  <option>Wedding</option>
                  <option>Private Party</option>
                  <option>Golf Tournament</option>
                  <option>Other</option>
                </select>
              </div>

              <div>
                <label className="block text-sm font-medium mb-2">Event Details</label>
                <textarea
                  rows="5"
                  placeholder="Tell us about your event"
                  className="w-full bg-black border border-zinc-700 rounded-2xl px-5 py-4 focus:outline-none focus:border-green-400"
                ></textarea>
              </div>

              <button
                type="submit"
                className="w-full bg-green-500 hover:bg-green-400 text-black font-bold py-4 rounded-2xl transition shadow-lg"
              >
                Submit Inquiry
              </button>
            </form>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t border-zinc-800 bg-black py-8">
        <div className="max-w-7xl mx-auto px-6 flex flex-col md:flex-row items-center justify-between gap-4">
          <div>
            <h3 className="text-xl font-bold">PSL Mobile Golf Simulator</h3>
            <p className="text-zinc-500 text-sm">Premium Mobile Golf Entertainment</p>
          </div>

          <div className="flex gap-6 text-zinc-400 text-sm">
            <a href="#home" className="hover:text-green-400">Home</a>
            <a href="#services" className="hover:text-green-400">Services</a>
            <a href="#contact" className="hover:text-green-400">Contact</a>
          </div>
        </div>
      </footer>
    </div>
  )
}
