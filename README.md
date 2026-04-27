import React from "react";
import { motion } from "framer-motion";

function Icon({ name, className = "w-6 h-6" }) {
  const commonProps = {
    className,
    viewBox: "0 0 24 24",
    fill: "none",
    stroke: "currentColor",
    strokeWidth: "2",
    strokeLinecap: "round",
    strokeLinejoin: "round",
    ariaHidden: "true"
  };

  const icons = {
    heart: (
      <svg {...commonProps}>
        <path d="M19.5 12.6 12 20l-7.5-7.4A5 5 0 0 1 12 6a5 5 0 0 1 7.5 6.6Z" />
        <path d="M12 6c1.1-2 3.6-2.7 5.4-1.3" />
      </svg>
    ),
    map: (
      <svg {...commonProps}>
        <path d="M12 21s7-5.3 7-12a7 7 0 0 0-14 0c0 6.7 7 12 7 12Z" />
        <circle cx="12" cy="9" r="2.5" />
      </svg>
    ),
    users: (
      <svg {...commonProps}>
        <path d="M16 21v-2a4 4 0 0 0-4-4H6a4 4 0 0 0-4 4v2" />
        <circle cx="9" cy="7" r="4" />
        <path d="M22 21v-2a4 4 0 0 0-3-3.8" />
        <path d="M16 3.2a4 4 0 0 1 0 7.6" />
      </svg>
    ),
    coins: (
      <svg {...commonProps}>
        <ellipse cx="12" cy="6" rx="7" ry="3" />
        <path d="M5 6v6c0 1.7 3.1 3 7 3s7-1.3 7-3V6" />
        <path d="M5 12v6c0 1.7 3.1 3 7 3s7-1.3 7-3v-6" />
      </svg>
    ),
    graduation: (
      <svg {...commonProps}>
        <path d="M22 10 12 5 2 10l10 5 10-5Z" />
        <path d="M6 12.5V16c0 1.7 2.7 3 6 3s6-1.3 6-3v-3.5" />
        <path d="M22 10v6" />
      </svg>
    ),
    sprout: (
      <svg {...commonProps}>
        <path d="M12 22V12" />
        <path d="M12 12C8 12 5 9 5 5c4 0 7 3 7 7Z" />
        <path d="M12 14c4 0 7-3 7-7-4 0-7 3-7 7Z" />
      </svg>
    ),
    phone: (
      <svg {...commonProps}>
        <path d="M22 16.9v3a2 2 0 0 1-2.2 2 19.8 19.8 0 0 1-8.6-3.1 19.5 19.5 0 0 1-6-6A19.8 19.8 0 0 1 2.1 4.2 2 2 0 0 1 4.1 2h3a2 2 0 0 1 2 1.7c.1 1 .4 2 .7 2.9a2 2 0 0 1-.5 2.1L8.1 9.9a16 16 0 0 0 6 6l1.2-1.2a2 2 0 0 1 2.1-.5c.9.3 1.9.6 2.9.7a2 2 0 0 1 1.7 2Z" />
      </svg>
    ),
    mail: (
      <svg {...commonProps}>
        <rect x="3" y="5" width="18" height="14" rx="2" />
        <path d="m3 7 9 6 9-6" />
      </svg>
    ),
    arrow: (
      <svg {...commonProps}>
        <path d="M5 12h14" />
        <path d="m13 5 7 7-7 7" />
      </svg>
    ),
    check: (
      <svg {...commonProps}>
        <circle cx="12" cy="12" r="10" />
        <path d="m9 12 2 2 4-5" />
      </svg>
    ),
    landmark: (
      <svg {...commonProps}>
        <path d="M3 22h18" />
        <path d="M6 18V9" />
        <path d="M10 18V9" />
        <path d="M14 18V9" />
        <path d="M18 18V9" />
        <path d="M4 9h16" />
        <path d="M12 2 3 7h18l-9-5Z" />
      </svg>
    ),
    book: (
      <svg {...commonProps}>
        <path d="M4 19.5A2.5 2.5 0 0 1 6.5 17H20" />
        <path d="M4 4.5A2.5 2.5 0 0 1 6.5 2H20v20H6.5A2.5 2.5 0 0 1 4 19.5v-15Z" />
      </svg>
    )
  };

  return icons[name] || icons.heart;
}

export default function WebsiteKampungZakatJember() {
  const programs = [
    {
      iconName: "coins",
      title: "Pengelolaan Zakat",
      text: "Menghimpun dan menyalurkan zakat, infak, dan sedekah untuk warga yang berhak menerima manfaat."
    },
    {
      iconName: "sprout",
      title: "Pemberdayaan Ekonomi",
      text: "Mendorong usaha warga melalui pelatihan, pendampingan, dan bantuan produktif sesuai kebutuhan lokal."
    },
    {
      iconName: "graduation",
      title: "Pendidikan dan Pembinaan",
      text: "Meningkatkan pemahaman masyarakat tentang zakat, kemandirian, dan penguatan kapasitas keluarga."
    },
    {
      iconName: "users",
      title: "Kolaborasi Lembaga",
      text: "Menghubungkan masyarakat, pengelola zakat, pemerintah, LAZ, dan relawan agar program lebih terarah."
    }
  ];

  const stats = [
    { number: "2018", label: "Tahun peresmian program" },
    { number: "4+", label: "Fokus pemberdayaan warga" },
    { number: "Dusun Paceh", label: "Lokasi kampung binaan" }
  ];

  const steps = [
    "Pemetaan kebutuhan warga dan calon penerima manfaat.",
    "Penghimpunan zakat, infak, sedekah, dan dukungan mitra.",
    "Penyaluran bantuan konsumtif dan produktif secara terarah.",
    "Pendampingan usaha, edukasi zakat, dan evaluasi program."
  ];

  const trustPoints = [
    "Transparan dalam pengelolaan dana sosial.",
    "Berbasis kebutuhan nyata masyarakat.",
    "Mendorong zakat produktif dan pendampingan warga.",
    "Terbuka untuk kerja sama lembaga dan relawan."
  ];

  return (
    <main className="min-h-screen bg-[#f7f7ef] text-slate-900">
      <section className="relative overflow-hidden bg-gradient-to-br from-emerald-900 via-emerald-800 to-lime-800 text-white">
        <div className="absolute inset-0 opacity-20 bg-[radial-gradient(circle_at_top_left,_white,_transparent_35%)]" />
        <div className="relative max-w-7xl mx-auto px-6 py-6 flex items-center justify-between">
          <div className="flex items-center gap-3">
            <div className="w-11 h-11 rounded-2xl bg-white/15 flex items-center justify-center shadow-lg">
              <Icon name="heart" className="w-6 h-6" />
            </div>
            <div>
              <p className="font-bold leading-tight">Kampung Zakat Jember</p>
              <p className="text-xs text-emerald-100">Dusun Paceh, Jambearum</p>
            </div>
          </div>
          <nav className="hidden md:flex gap-7 text-sm text-emerald-50">
            <a href="#tentang" className="hover:text-white">Tentang</a>
            <a href="#program" className="hover:text-white">Program</a>
            <a href="#alur" className="hover:text-white">Alur</a>
            <a href="#kontak" className="hover:text-white">Kontak</a>
          </nav>
        </div>

        <div className="relative max-w-7xl mx-auto px-6 py-20 md:py-28 grid md:grid-cols-2 gap-12 items-center">
          <motion.div initial={{ opacity: 0, y: 24 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 0.6 }}>
            <div className="inline-flex items-center gap-2 rounded-full bg-white/12 px-4 py-2 text-sm text-emerald-50 mb-6">
              <Icon name="map" className="w-4 h-4" />
              Dusun Paceh, Desa Jambearum, Kecamatan Sumberjambe, Jember
            </div>
            <h1 className="text-4xl md:text-6xl font-extrabold tracking-tight leading-tight">
              Zakat yang Menguatkan Warga dan Menggerakkan Desa
            </h1>
            <p className="mt-6 text-lg text-emerald-50 leading-8 max-w-xl">
              Kampung Zakat Jember hadir sebagai ruang kolaborasi untuk pengelolaan zakat, pemberdayaan ekonomi, dan peningkatan kualitas hidup masyarakat Dusun Paceh.
            </p>
            <div className="mt-8 flex flex-col sm:flex-row gap-4">
              <a href="#kontak" className="inline-flex items-center justify-center gap-2 rounded-2xl bg-white text-emerald-900 px-6 py-3 font-semibold shadow-lg hover:bg-emerald-50">
                Hubungi Pengelola <Icon name="arrow" className="w-4 h-4" />
              </a>
              <a href="#program" className="inline-flex items-center justify-center gap-2 rounded-2xl bg-white/10 border border-white/25 px-6 py-3 font-semibold hover:bg-white/15">
                Lihat Program
              </a>
            </div>
          </motion.div>

          <motion.div initial={{ opacity: 0, scale: 0.95 }} animate={{ opacity: 1, scale: 1 }} transition={{ duration: 0.7, delay: 0.1 }} className="bg-white/12 backdrop-blur rounded-[2rem] p-5 shadow-2xl border border-white/20">
            <div className="bg-white text-slate-900 rounded-[1.5rem] p-6 md:p-8">
              <div className="w-full h-56 rounded-3xl bg-gradient-to-br from-lime-100 to-emerald-100 flex items-center justify-center mb-6">
                <Icon name="landmark" className="w-24 h-24 text-emerald-800" />
              </div>
              <h2 className="text-2xl font-bold mb-3">Tentang Kampung Zakat</h2>
              <p className="text-slate-600 leading-7">
                Program ini berfokus pada penguatan masyarakat melalui dana zakat yang dikelola secara terarah. Kegiatan diarahkan untuk membantu warga, meningkatkan pemahaman zakat, dan mendukung kemandirian ekonomi.
              </p>
            </div>
          </motion.div>
        </div>
      </section>

      <section className="max-w-7xl mx-auto px-6 -mt-10 relative z-10">
        <div className="grid md:grid-cols-3 gap-5">
          {stats.map((item) => (
            <div key={item.label} className="bg-white rounded-3xl p-6 shadow-xl border border-slate-100">
              <p className="text-3xl font-extrabold text-emerald-800">{item.number}</p>
              <p className="mt-2 text-slate-600">{item.label}</p>
            </div>
          ))}
        </div>
      </section>

      <section id="tentang" className="max-w-7xl mx-auto px-6 py-20 grid md:grid-cols-2 gap-10 items-center">
        <div>
          <p className="text-emerald-800 font-semibold mb-3">Tentang Kami</p>
          <h2 className="text-3xl md:text-4xl font-extrabold leading-tight mb-5">
            Mengubah zakat menjadi gerakan pemberdayaan masyarakat.
          </h2>
          <p className="text-slate-600 leading-8 mb-5">
            Kampung Zakat Terpadu Dusun Paceh menjadi contoh program berbasis kolaborasi. Program ini menyalurkan bantuan dan mendorong warga agar punya peluang usaha, pengetahuan, serta akses pendampingan.
          </p>
          <p className="text-slate-600 leading-8">
            Website ini dapat digunakan untuk profil lembaga, publikasi program, laporan kegiatan, galeri, dan informasi donasi.
          </p>
        </div>
        <div className="grid gap-4">
          {trustPoints.map((text) => (
            <div key={text} className="flex gap-3 bg-white rounded-2xl p-5 shadow-sm border border-slate-100">
              <Icon name="check" className="w-6 h-6 text-emerald-700 shrink-0" />
              <p className="text-slate-700">{text}</p>
            </div>
          ))}
        </div>
      </section>

      <section id="program" className="bg-white py-20">
        <div className="max-w-7xl mx-auto px-6">
          <div className="max-w-2xl mb-10">
            <p className="text-emerald-800 font-semibold mb-3">Program Utama</p>
            <h2 className="text-3xl md:text-4xl font-extrabold leading-tight">
              Fokus kegiatan yang bisa langsung dirasakan masyarakat.
            </h2>
          </div>
          <div className="grid md:grid-cols-4 gap-5">
            {programs.map((item) => (
              <div key={item.title} className="rounded-3xl p-6 bg-[#f7f7ef] border border-slate-100 hover:shadow-xl transition-shadow">
                <div className="w-14 h-14 rounded-2xl bg-emerald-800 text-white flex items-center justify-center mb-5">
                  <Icon name={item.iconName} className="w-7 h-7" />
                </div>
                <h3 className="text-xl font-bold mb-3">{item.title}</h3>
                <p className="text-slate-600 leading-7">{item.text}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      <section id="alur" className="max-w-7xl mx-auto px-6 py-20">
        <div className="grid md:grid-cols-2 gap-12 items-start">
          <div>
            <p className="text-emerald-800 font-semibold mb-3">Alur Program</p>
            <h2 className="text-3xl md:text-4xl font-extrabold leading-tight mb-5">
              Program berjalan dari pemetaan sampai pendampingan.
            </h2>
            <p className="text-slate-600 leading-8">
              Alur ini membantu pengelola menjelaskan proses kerja kepada donatur, mitra, dan masyarakat. Data program dapat diperbarui sesuai laporan kegiatan terbaru.
            </p>
          </div>
          <div className="space-y-4">
            {steps.map((step, index) => (
              <div key={step} className="bg-white rounded-3xl p-5 shadow-sm border border-slate-100 flex gap-4">
                <div className="w-10 h-10 rounded-2xl bg-emerald-800 text-white flex items-center justify-center font-bold shrink-0">
                  {index + 1}
                </div>
                <p className="text-slate-700 leading-7">{step}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      <section className="bg-emerald-900 text-white py-20">
        <div className="max-w-7xl mx-auto px-6 grid md:grid-cols-3 gap-6">
          <div className="md:col-span-2">
            <p className="text-emerald-100 font-semibold mb-3">Mari Berkolaborasi</p>
            <h2 className="text-3xl md:text-4xl font-extrabold leading-tight mb-5">
              Dukung Kampung Zakat Jember melalui zakat, infak, sedekah, program sosial, atau pendampingan keahlian.
            </h2>
            <p className="text-emerald-50 leading-8 max-w-2xl">
              Setiap dukungan dapat diarahkan untuk bantuan warga, pelatihan usaha, edukasi zakat, dan kegiatan sosial yang berdampak bagi Dusun Paceh.
            </p>
          </div>
          <div className="bg-white text-slate-900 rounded-3xl p-6 shadow-xl">
            <Icon name="book" className="w-10 h-10 text-emerald-800 mb-4" />
            <h3 className="text-xl font-bold mb-3">Butuh halaman laporan?</h3>
            <p className="text-slate-600 leading-7 mb-5">
              Tambahkan halaman laporan dana, dokumentasi kegiatan, dan daftar mitra agar website lebih dipercaya.
            </p>
            <a href="#kontak" className="inline-flex items-center gap-2 font-semibold text-emerald-800">
              Tambahkan Kontak <Icon name="arrow" className="w-4 h-4" />
            </a>
          </div>
        </div>
      </section>

      <section id="kontak" className="max-w-7xl mx-auto px-6 py-20">
        <div className="bg-white rounded-[2rem] p-8 md:p-12 shadow-xl border border-slate-100 grid md:grid-cols-2 gap-10">
          <div>
            <p className="text-emerald-800 font-semibold mb-3">Kontak</p>
            <h2 className="text-3xl md:text-4xl font-extrabold leading-tight mb-5">
              Hubungi Pengelola Kampung Zakat Jember
            </h2>
            <p className="text-slate-600 leading-8">
              Silakan sesuaikan nomor WhatsApp, email, dan alamat detail di bagian ini sebelum website dipublikasikan.
            </p>
          </div>
          <div className="space-y-4">
            <div className="flex gap-4 rounded-2xl bg-[#f7f7ef] p-5">
              <Icon name="map" className="w-6 h-6 text-emerald-800 shrink-0" />
              <div>
                <p className="font-semibold">Alamat</p>
                <p className="text-slate-600">Dusun Paceh, Desa Jambearum, Kecamatan Sumberjambe, Kabupaten Jember</p>
              </div>
            </div>
            <div className="flex gap-4 rounded-2xl bg-[#f7f7ef] p-5">
              <Icon name="phone" className="w-6 h-6 text-emerald-800 shrink-0" />
              <div>
                <p className="font-semibold">WhatsApp</p>
                <p className="text-slate-600">08xx-xxxx-xxxx</p>
              </div>
            </div>
            <div className="flex gap-4 rounded-2xl bg-[#f7f7ef] p-5">
              <Icon name="mail" className="w-6 h-6 text-emerald-800 shrink-0" />
              <div>
                <p className="font-semibold">Email</p>
                <p className="text-slate-600">kampungzakatjember@email.com</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      <footer className="bg-slate-950 text-white py-8">
        <div className="max-w-7xl mx-auto px-6 flex flex-col md:flex-row justify-between gap-4 text-sm text-slate-300">
          <p>© 2026 Kampung Zakat Jember. Dusun Paceh, Jambearum.</p>
          <p>Website profil dan informasi program pemberdayaan masyarakat.</p>
        </div>
      </footer>
    </main>
  );
}
