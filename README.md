# aapno-pilani-portfolio
A modern luxury portfolio website built for Instagram creator @aapno_pilani with cinematic visuals, premium branding, and social media showcase
export default function AapnoPilaniPortfolio() { const reels = [ { title: 'Luxury Street Reel', views: '1.2M Views', video: 'https://www.w3schools.com/html/mov_bbb.mp4', }, { title: 'Pilani Cinematic', views: '850K Views', video: 'https://www.w3schools.com/html/movie.mp4', }, ];

return ( <div className="min-h-screen bg-black text-white overflow-hidden font-sans"> {/* Loading Screen */} <div className="fixed inset-0 bg-black z-50 flex items-center justify-center animate-pulse pointer-events-none"> <h1 className="text-5xl md:text-7xl font-black tracking-[8px] text-yellow-400"> AAPNO PILANI </h1> </div>

{/* Background Music */}
  <audio autoPlay loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mp3" />
  </audio>

  {/* Hero Section */}
  <section className="relative min-h-screen flex items-center justify-center px-4 overflow-hidden">
    <div className="absolute inset-0">
      <img
        src="https://images.unsplash.com/photo-1506744038136-46273834b3fb"
        alt="background"
        className="w-full h-full object-cover opacity-40 scale-110"
      />
      <div className="absolute inset-0 bg-black/80"></div>
    </div>

    <div className="absolute top-0 left-0 w-[400px] h-[400px] bg-yellow-400/20 blur-3xl rounded-full"></div>
    <div className="absolute bottom-0 right-0 w-[350px] h-[350px] bg-red-500/20 blur-3xl rounded-full"></div>

    <div className="relative z-10 max-w-6xl grid md:grid-cols-2 gap-12 items-center">
      <div className="text-center md:text-left">

      <p className="uppercase tracking-[6px] text-yellow-400 text-sm mb-5 animate-bounce">
        Premium Digital Creator
      </p>

      <h1 className="text-6xl md:text-8xl font-black leading-tight">
        Aapno <span className="text-yellow-400">Pilani</span>
      </h1>

      <p className="mt-8 text-gray-300 text-lg md:text-2xl leading-relaxed max-w-3xl mx-auto">
        Viral reels • Rajasthan vibes • Luxury cinematic storytelling.
      </p>

      <div className="flex gap-4 justify-center flex-wrap mt-10">
        <a
          href="https://instagram.com/aapno_pilani"
          target="_blank"
          className="px-8 py-4 bg-yellow-400 text-black rounded-2xl font-bold shadow-2xl hover:scale-110 transition duration-500"
        >
          Instagram Profile
        </a>

        <a
          href="https://wa.me/919460225031"
          target="_blank"
          className="px-8 py-4 border border-white rounded-2xl hover:bg-white hover:text-black transition duration-500"
        >
          WhatsApp Contact
        </a>
      </div>

      <div className="mt-14 flex justify-center gap-12 flex-wrap">
        <div>
          <h2 className="text-5xl font-black text-yellow-400">26K+</h2>
          <p className="text-gray-400 mt-2">Followers</p>
        </div>

        <div>
          <h2 className="text-5xl font-black text-yellow-400">500+</h2>
          <p className="text-gray-400 mt-2">Luxury Reels</p>
        </div>
      </div>
    </div>

      <div className="flex justify-center">
        <div className="relative">
          <div className="absolute inset-0 bg-yellow-400/20 blur-3xl rounded-full"></div>
          <img
            src="/mnt/data/1000070088.png"
            alt="Aapno Pilani"
            className="relative w-[300px] md:w-[380px] h-[500px] object-cover rounded-[40px] border border-yellow-400/30 shadow-2xl hover:scale-105 transition duration-500"
          />
        </div>
      </div>
    </div>
  </section>

  {/* Reels Section */}
  <section className="py-24 px-4 bg-zinc-950 border-t border-white/10">
    <div className="max-w-7xl mx-auto">
      <div className="text-center mb-16">
        <p className="text-yellow-400 uppercase tracking-[5px] text-sm">
          Trending Content
        </p>
        <h2 className="text-5xl md:text-6xl font-black mt-4">
          Video Reels Showcase
        </h2>
      </div>

      <div className="grid md:grid-cols-2 gap-10">
        {reels.map((reel, index) => (
          <div
            key={index}
            className="bg-black border border-white/10 rounded-3xl overflow-hidden shadow-2xl hover:-translate-y-2 transition duration-500"
          >
            <video
              src={reel.video}
              controls
              muted
              loop
              className="w-full h-[420px] object-cover"
            />

            <div className="p-6">
              <h3 className="text-3xl font-bold">{reel.title}</h3>
              <p className="text-yellow-400 mt-3">{reel.views}</p>
            </div>
          </div>
        ))}
      </div>
    </div>
  </section>

  {/* Instagram Feed */}
  <section className="py-24 px-4 bg-black border-t border-white/10">
    <div className="max-w-7xl mx-auto text-center">
      <p className="text-yellow-400 uppercase tracking-[5px] text-sm">
        Social Presence
      </p>

      <h2 className="text-5xl md:text-6xl font-black mt-4 mb-16">
        Instagram Feed
      </h2>

      <div className="grid grid-cols-2 md:grid-cols-4 gap-6">
        <img src="/mnt/data/1000070088.png" className="rounded-3xl h-[260px] object-cover hover:scale-105 transition duration-500" />
        <img src="/mnt/data/1000068122.png" className="rounded-3xl h-[260px] object-cover hover:scale-105 transition duration-500" />
        <img src="/mnt/data/1000070088.png" className="rounded-3xl h-[260px] object-cover hover:scale-105 transition duration-500" />
        <img src="/mnt/data/1000068122.png" className="rounded-3xl h-[260px] object-cover hover:scale-105 transition duration-500" />
        <img src="/mnt/data/1000070088.png" className="rounded-3xl h-[260px] object-cover hover:scale-105 transition duration-500" />
        <img src="/mnt/data/1000060370.jpg" className="rounded-3xl h-[260px] object-cover hover:scale-105 transition duration-500" />
      </div>
    </div>
  </section>

  {/* Admin Section */}
  <section className="py-24 px-4 bg-zinc-950 border-t border-white/10 text-center">
    <p className="text-yellow-400 uppercase tracking-[5px] text-sm">
      Creator Dashboard
    </p>

    <h2 className="text-5xl md:text-6xl font-black mt-4">
      Admin Panel Ready
    </h2>

    <p className="text-gray-400 text-lg max-w-3xl mx-auto mt-8 leading-relaxed">
      Future-ready premium admin panel integration for managing reels, gallery,
      analytics, follower growth, and creator branding.
    </p>
  </section>

  {/* Footer */}
  <footer className="py-10 border-t border-white/10 bg-black text-center">
    <h2 className="text-3xl font-bold text-yellow-400">@aapno_pilani</h2>
    <p className="text-gray-500 mt-3">
      Designed for the digital face of Pilani ✨
    </p>
  </footer>
</div>

); }
