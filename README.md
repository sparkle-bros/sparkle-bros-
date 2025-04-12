import Link from "next/link"

export default function HomePage() {
  return (
    <div className="min-h-screen bg-white text-gray-800 font-sans">
      <header className="bg-blue-900 text-white p-6 shadow-md">
        <div className="max-w-6xl mx-auto flex justify-between items-center">
          <div>
            <h1 className="text-3xl font-bold">✨ Sparkle Bros ✨</h1>
            <p className="text-sm">Mobile Car Cleaning That Comes to You!</p>
          </div>
          <nav className="hidden md:block">
            <ul className="flex space-x-6">
              <li>
                <a href="#services" className="hover:text-blue-200 transition">
                  Services
                </a>
              </li>
              <li>
                <a href="#how-it-works" className="hover:text-blue-200 transition">
                  How It Works
                </a>
              </li>
              <li>
                <a href="#testimonials" className="hover:text-blue-200 transition">
                  Testimonials
                </a>
              </li>
              <li>
                <a href="#contact" className="hover:text-blue-200 transition">
                  Contact
                </a>
              </li>
            </ul>
          </nav>
        </div>
      </header>

      <main className="p-6 max-w-6xl mx-auto">
        {/* Hero Section */}
        <section className="py-12 text-center">
          <h2 className="text-4xl font-bold mb-4">Professional Mobile Car Cleaning</h2>
          <p className="text-xl mb-8 max-w-3xl mx-auto">
            We bring the car wash to you! Professional detailing services at your home or office.
          </p>
          <Link
            href="/book"
            className="bg-blue-900 text-white px-8 py-3 rounded-full text-lg font-semibold hover:bg-blue-800 transition inline-block"
          >
            Book Now
          </Link>
        </section>

        {/* Services Section */}
        <section id="services" className="mb-16">
          <h2 className="text-3xl font-semibold mb-8 text-center">🚗 Car Cleaning Packages</h2>

          <div className="grid md:grid-cols-3 gap-6">
            <div className="border rounded-2xl p-6 shadow hover:shadow-lg transition">
              <h3 className="text-2xl font-bold mb-3">🥈 Silver – $45</h3>
              <p className="text-gray-600 mb-4">Perfect for a quick exterior refresh</p>
              <ul className="list-disc list-inside space-y-2 mb-6">
                <li>Hand-wash exterior</li>
                <li>Wheels cleaned & tires dressed</li>
                <li>Windows & mirrors cleaned</li>
                <li>Exterior plastic/trim protected</li>
              </ul>
              <Link
                href="/book?package=Silver - $45"
                className="block text-center bg-gray-100 hover:bg-gray-200 text-blue-900 font-semibold py-2 rounded-lg transition"
              >
                Select Package
              </Link>
            </div>

            <div className="border rounded-2xl p-6 shadow hover:shadow-lg transition">
              <h3 className="text-2xl font-bold mb-3">🥇 Gold – $45</h3>
              <p className="text-gray-600 mb-4">Interior refresh for a clean cabin</p>
              <ul className="list-disc list-inside space-y-2 mb-6">
                <li>Full interior vacuum</li>
                <li>Dashboard & console cleaned</li>
                <li>Door panels & seats wiped down</li>
                <li>Interior glass cleaned</li>
                <li>Air freshener applied</li>
              </ul>
              <Link
                href="/book?package=Gold - $45"
                className="block text-center bg-gray-100 hover:bg-gray-200 text-blue-900 font-semibold py-2 rounded-lg transition"
              >
                Select Package
              </Link>
            </div>

            <div className="border rounded-2xl p-6 shadow-md hover:shadow-lg transition bg-blue-50">
              <div className="absolute -mt-8 -mr-4 right-0 text-sm bg-blue-900 text-white px-3 py-1 rounded-full">
                Most Popular
              </div>
              <h3 className="text-2xl font-bold mb-3">🔥 Platinum – $85</h3>
              <p className="text-gray-600 mb-4">Complete interior & exterior detail</p>
              <ul className="list-disc list-inside space-y-2 mb-6">
                <li>Full Silver & Gold packages included</li>
                <li>Deep clean of all interior surfaces</li>
                <li>Leather conditioning (if applicable)</li>
                <li>Carpet & upholstery shampoo</li>
                <li>Premium wax protection</li>
                <li>Headlight restoration</li>
              </ul>
              <Link
                href="/book?package=Platinum - $85"
                className="block text-center bg-blue-900 hover:bg-blue-800 text-white font-semibold py-2 rounded-lg transition"
              >
                Select Package
              </Link>
            </div>
          </div>
        </section>

        {/* How It Works Section */}
        <section id="how-it-works" className="mb-16">
          <h2 className="text-3xl font-semibold mb-8 text-center">How It Works</h2>

          <div className="grid md:grid-cols-3 gap-8">
            <div className="text-center">
              <div className="bg-blue-900 text-white w-12 h-12 rounded-full flex items-center justify-center text-xl font-bold mx-auto mb-4">
                1
              </div>
              <h3 className="text-xl font-semibold mb-2">Book Online</h3>
              <p>
                Schedule your appointment through our easy online booking system. Select your package and preferred
                time.
              </p>
            </div>

            <div className="text-center">
              <div className="bg-blue-900 text-white w-12 h-12 rounded-full flex items-center justify-center text-xl font-bold mx-auto mb-4">
                2
              </div>
              <h3 className="text-xl font-semibold mb-2">We Come To You</h3>
              <p>Our mobile team arrives at your location with all equipment and eco-friendly supplies needed.</p>
            </div>

            <div className="text-center">
              <div className="bg-blue-900 text-white w-12 h-12 rounded-full flex items-center justify-center text-xl font-bold mx-auto mb-4">
                3
              </div>
              <h3 className="text-xl font-semibold mb-2">Enjoy Your Clean Car</h3>
              <p>Relax while we transform your vehicle. No need to drive anywhere or wait in line!</p>
            </div>
          </div>
        </section>

        {/* Testimonials Section */}
        <section id="testimonials" className="mb-16">
          <h2 className="text-3xl font-semibold mb-8 text-center">What Our Customers Say</h2>

          <div className="grid md:grid-cols-3 gap-6">
            <div className="bg-gray-50 p-6 rounded-lg shadow">
              <div className="flex items-center mb-4">
                <div className="text-yellow-400 text-xl">★★★★★</div>
                <div className="ml-2 font-semibold">Michael T.</div>
              </div>
              <p className="italic">
                "These guys are amazing! They came to my office and detailed my car while I was working. Came back to a
                car that looked brand new!"
              </p>
            </div>

            <div className="bg-gray-50 p-6 rounded-lg shadow">
              <div className="flex items-center mb-4">
                <div className="text-yellow-400 text-xl">★★★★★</div>
                <div className="ml-2 font-semibold">Sarah K.</div>
              </div>
              <p className="italic">
                "I've tried several mobile detailers and Sparkle Bros is by far the best. Attention to detail is
                incredible and they're always on time."
              </p>
            </div>

            <div className="bg-gray-50 p-6 rounded-lg shadow">
              <div className="flex items-center mb-4">
                <div className="text-yellow-400 text-xl">★★★★★</div>
                <div className="ml-2 font-semibold">James R.</div>
              </div>
              <p className="italic">
                "The Platinum package is worth every penny! My 5-year-old SUV looks showroom new. Will definitely be a
                repeat customer."
              </p>
            </div>
          </div>
        </section>

        {/* Contact Section */}
        <section id="contact" className="mb-16">
          <h2 className="text-3xl font-semibold mb-8 text-center">Contact Us</h2>

          <div className="bg-gray-50 p-8 rounded-xl shadow-md max-w-2xl mx-auto text-center">
            <p className="mb-6">Have questions or need more information? Contact us or book your appointment now!</p>

            <div className="flex flex-col md:flex-row justify-center gap-4 mb-8">
              <a
                href="tel:9545591416"
                className="inline-flex items-center justify-center bg-white border border-gray-200 rounded-lg px-4 py-2 hover:bg-gray-50"
              >
                <span className="mr-2">📱</span> (954) 559-1416
              </a>
              <a
                href="mailto:joshuacomet74@gmail.com"
                className="inline-flex items-center justify-center bg-white border border-gray-200 rounded-lg px-4 py-2 hover:bg-gray-50"
              >
                <span className="mr-2">✉️</span> joshuacomet74@gmail.com
              </a>
            </div>

            <Link
              href="/book"
              className="bg-blue-900 text-white px-8 py-3 rounded-lg text-lg font-semibold hover:bg-blue-800 transition inline-block"
            >
              Book Your Appointment
            </Link>
          </div>
        </section>
      </main>

      <footer className="bg-blue-900 text-white py-8">
        <div className="max-w-6xl mx-auto px-6">
          <div className="grid md:grid-cols-3 gap-8">
            <div>
              <h3 className="text-xl font-bold mb-4">✨ Sparkle Bros ✨</h3>
              <p>
                Mobile car cleaning services that come to your home or workplace. Professional results without the
                hassle.
              </p>
            </div>

            <div>
              <h3 className="text-xl font-bold mb-4">Contact Us</h3>
              <p className="mb-2">📱 (954) 559-1416</p>
              <p className="mb-2">✉️ joshuacomet74@gmail.com</p>
              <p>🚗 Serving the greater metro area</p>
            </div>

            <div>
              <h3 className="text-xl font-bold mb-4">Hours</h3>
              <p className="mb-2">Monday - Friday: 8am - 6pm</p>
              <p className="mb-2">Saturday: 9am - 5pm</p>
              <p>Sunday: 10am - 3pm</p>
            </div>
          </div>

          <div className="border-t border-blue-800 mt-8 pt-8 text-center">
            <p>&copy; {new Date().getFullYear()} Sparkle Bros Mobile Car Cleaning. All rights reserved.</p>
          </div>
        </div>
      </footer>
    </div>
  )
}
