html
<!DOCTYPE html>
<html lang="ms" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Isa Wiring - Pakar Pendawaian, Aircond, Autogate & CCTV</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#fffbeb',
                            100: '#fef3c7',
                            200: '#fde68a',
                            300: '#fcd34d',
                            400: '#fbbf24',
                            500: '#f59e0b', /* Warna utama kuning elektrik */
                            600: '#d97706',
                            700: '#b45309',
                            800: '#92400e',
                            900: '#78350f',
                        },
                        dark: {
                            50: '#f8fafc',
                            100: '#f1f5f9',
                            800: '#1e293b',
                            900: '#0f172a',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Kesan transisi lancar */
        .transition-all {
            transition: all 0.3s ease-in-out;
        }
        /* Bar skrol tersuai untuk rupa premium */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #1e293b;
        }
        ::-webkit-scrollbar-thumb {
            background: #fbbf24;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #d97706;
        }
    </style>
</head>
<body class="bg-dark-50 text-dark-900 font-sans antialiased selection:bg-brand-400 selection:text-dark-900">

    <!-- Bar Informasi Atas -->
    <div class="bg-dark-900 text-white py-2 px-4 text-xs md:text-sm border-b border-brand-500/20">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-2">
            <div class="flex items-center gap-4">
                <span class="flex items-center gap-1">
                    <svg class="w-4 h-4 text-brand-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
                    Kawasan Perkhidmatan: Selangor, Kuala Lumpur & Negeri Sembilan
                </span>
            </div>
            <div class="flex items-center gap-4">
                <span class="flex items-center gap-1">
                    <svg class="w-4 h-4 text-brand-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                    Isnin - Ahad (8:00 AM - 10:00 PM)
                </span>
            </div>
        </div>
    </div>

    <!-- Kepala Laman (Header Navigation) -->
    <header class="sticky top-0 z-50 bg-white/95 backdrop-blur-md shadow-md transition-all">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                
                <!-- Logo & Nama Brand bersebelahan -->
                <a href="#home" class="flex items-center gap-3 group">
                    <div class="bg-dark-900 p-2.5 rounded-xl border border-brand-400 shadow-inner group-hover:scale-105 transition-transform">
                        <!-- Logo Kilat SVG Tersuai -->
                        <svg class="w-8 h-8 text-brand-400 animate-pulse" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
                            <polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polygon>
                        </svg>
                    </div>
                    <div class="flex flex-col">
                        <span class="text-2xl font-black tracking-wider text-dark-900 uppercase">
                            Isa <span class="text-brand-500">Wiring</span>
                        </span>
                        <span class="text-[10px] tracking-widest text-gray-500 uppercase font-bold -mt-1">Pakar Elektrikal Anda</span>
                    </div>
                </a>

                <!-- Menu Desktop -->
                <nav class="hidden md:flex items-center gap-8 font-semibold text-gray-700">
                    <a href="#home" class="hover:text-brand-600 transition-colors">Utama</a>
                    <a href="#perkhidmatan" class="hover:text-brand-600 transition-colors">Perkhidmatan</a>
                    <a href="#hasil-kerja" class="hover:text-brand-600 transition-colors">Hasil Kerja</a>
                    <a href="https://wa.me/60189141560" target="_blank" class="bg-brand-500 hover:bg-brand-600 text-dark-900 px-5 py-2.5 rounded-xl flex items-center gap-2 shadow-lg hover:shadow-brand-500/20 active:scale-95 transition-all">
                        <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397.01 12.008.01c3.202.001 6.212 1.246 8.477 3.513 2.266 2.268 3.507 5.28 3.505 8.484-.004 6.657-5.34 11.997-11.953 11.997-2.005-.001-3.973-.502-5.724-1.457L0 24zm6.59-4.846c1.6.95 3.188 1.449 4.825 1.451 5.436 0 9.86-4.37 9.864-9.799.002-2.63-1.023-5.101-2.885-6.963C16.588 1.981 14.115.957 11.5.957c-5.442 0-9.87 4.372-9.874 9.802-.001 1.774.502 3.509 1.457 5.032l-1.012 3.702 3.813-1.002z"/></svg>
                        Hubungi Kami
                    </a>
                </nav>

                <!-- Butang Menu Mobil -->
                <button id="mobile-menu-btn" class="md:hidden p-2 rounded-lg text-gray-700 hover:bg-gray-100 focus:outline-none" aria-label="Toggle Menu">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"/></svg>
                </button>
            </div>
        </div>

        <!-- Menu Mobil -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100 px-4 py-4 space-y-3 shadow-lg">
            <a href="#home" class="block py-2 px-3 rounded-lg hover:bg-brand-50 text-gray-800 font-medium">Utama</a>
            <a href="#perkhidmatan" class="block py-2 px-3 rounded-lg hover:bg-brand-50 text-gray-800 font-medium">Perkhidmatan</a>
            <a href="#hasil-kerja" class="block py-2 px-3 rounded-lg hover:bg-brand-50 text-gray-800 font-medium">Hasil Kerja</a>
            <a href="https://wa.me/60189141560" target="_blank" class="w-full bg-brand-500 text-dark-900 py-3 rounded-xl flex items-center justify-center gap-2 font-bold shadow-md">
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397.01 12.008.01c3.202.001 6.212 1.246 8.477 3.513 2.266 2.268 3.507 5.28 3.505 8.484-.004 6.657-5.34 11.997-11.953 11.997-2.005-.001-3.973-.502-5.724-1.457L0 24zm6.59-4.846c1.6.95 3.188 1.449 4.825 1.451 5.436 0 9.86-4.37 9.864-9.799.002-2.63-1.023-5.101-2.885-6.963C16.588 1.981 14.115.957 11.5.957c-5.442 0-9.87 4.372-9.874 9.802-.001 1.774.502 3.509 1.457 5.032l-1.012 3.702 3.813-1.002z"/></svg>
                Hubungi Sekarang
            </a>
        </div>
    </header>

    <!-- Seksyen Hero -->
    <section id="home" class="relative bg-dark-900 text-white overflow-hidden py-20 lg:py-32">
        <div class="absolute inset-0 opacity-10 bg-[radial-gradient(#fbbf24_1px,transparent_1px)] [background-size:16px_16px]"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                    <span class="inline-flex items-center gap-2 bg-brand-500/10 text-brand-400 px-4 py-2 rounded-full text-sm font-semibold border border-brand-500/20">
                        <span class="w-2 h-2 rounded-full bg-brand-400 animate-ping"></span>
                        Servis Pantas & Profesional
                    </span>
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-black tracking-tight leading-none">
                        Selesaikan Masalah Elektrikal Rumah Anda Dengan <span class="text-brand-400">Selamat</span>
                    </h1>
                    <p class="text-gray-300 text-lg md:text-xl max-w-2xl mx-auto lg:mx-0">
                        Kami menyediakan khidmat pakar untuk **Pendawaian (Wiring)**, pemasangan **Aircond**, pemasangan sistem **Autogate**, dan pemasangan kamera **CCTV** berdefinisi tinggi.
                    </p>
                    
                    <div class="flex flex-col sm:flex-row gap-4 justify-center lg:justify-start">
                        <a href="https://wa.me/60189141560?text=Salam%20Isa%20Wiring.%20Saya%20nak%20tanya%20mengenai%20servis%20anda." target="_blank" class="bg-brand-500 hover:bg-brand-600 text-dark-900 font-bold px-8 py-4 rounded-2xl flex items-center justify-center gap-3 shadow-xl shadow-brand-500/10 hover:shadow-brand-500/20 hover:scale-[1.02] active:scale-95 transition-all text-lg">
                            <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397.01 12.008.01c3.202.001 6.212 1.246 8.477 3.513 2.266 2.268 3.507 5.28 3.505 8.484-.004 6.657-5.34 11.997-11.953 11.997-2.005-.001-3.973-.502-5.724-1.457L0 24zm6.59-4.846c1.6.95 3.188 1.449 4.825 1.451 5.436 0 9.86-4.37 9.864-9.799.002-2.63-1.023-5.101-2.885-6.963C16.588 1.981 14.115.957 11.5.957c-5.442 0-9.87 4.372-9.874 9.802-.001 1.774.502 3.509 1.457 5.032l-1.012 3.702 3.813-1.002z"/></svg>
                            Hubungi Melalui WhatsApp
                        </a>
                        <a href="#perkhidmatan" class="border-2 border-gray-600 hover:border-brand-400 hover:text-brand-400 font-bold px-8 py-4 rounded-2xl flex items-center justify-center transition-colors text-lg">
                            Lihat Perkhidmatan
                        </a>
                    </div>
                </div>

                <!-- Widget Anggaran Pintar -->
                <div class="lg:col-span-5">
                    <div class="bg-dark-800 rounded-3xl p-6 sm:p-8 border border-gray-700 shadow-2xl relative">
                        <div class="absolute -top-3 -right-3 bg-brand-500 text-dark-900 text-xs font-black px-3 py-1 rounded-full uppercase tracking-wider shadow">
                            Sebut Harga Percuma
                        </div>
                        <h3 class="text-xl font-bold text-white mb-4">Dapatkan Anggaran Pantas</h3>
                        <p class="text-gray-400 text-sm mb-6">Pilih perkhidmatan yang diperlukan & hantar terus ke telefon kami.</p>
                        
                        <div class="space-y-4">
                            <div>
                                <label class="block text-xs font-bold text-gray-400 uppercase tracking-wider mb-2">Pilih Perkhidmatan</label>
                                <div class="grid grid-cols-2 gap-2">
                                    <button onclick="toggleService('Wiring')" id="btn-Wiring" class="service-selector-btn py-2.5 px-3 rounded-xl border border-gray-700 text-sm font-semibold bg-dark-900 hover:border-brand-500 text-gray-300 hover:text-white flex items-center gap-2 transition-all">
                                        <span class="w-2.5 h-2.5 rounded-full bg-gray-600 status-dot"></span> Wiring
                                    </button>
                                    <button onclick="toggleService('Aircond')" id="btn-Aircond" class="service-selector-btn py-2.5 px-3 rounded-xl border border-gray-700 text-sm font-semibold bg-dark-900 hover:border-brand-500 text-gray-300 hover:text-white flex items-center gap-2 transition-all">
                                        <span class="w-2.5 h-2.5 rounded-full bg-gray-600 status-dot"></span> Aircond
                                    </button>
                                    <button onclick="toggleService('Autogate')" id="btn-Autogate" class="service-selector-btn py-2.5 px-3 rounded-xl border border-gray-700 text-sm font-semibold bg-dark-900 hover:border-brand-500 text-gray-300 hover:text-white flex items-center gap-2 transition-all">
                                        <span class="w-2.5 h-2.5 rounded-full bg-gray-600 status-dot"></span> Autogate
                                    </button>
                                    <button onclick="toggleService('CCTV')" id="btn-CCTV" class="service-selector-btn py-2.5 px-3 rounded-xl border border-gray-700 text-sm font-semibold bg-dark-900 hover:border-brand-500 text-gray-300 hover:text-white flex items-center gap-2 transition-all">
                                        <span class="w-2.5 h-2.5 rounded-full bg-gray-600 status-dot"></span> CCTV
                                    </button>
                                </div>
                            </div>

                            <div>
                                <label for="client-name" class="block text-xs font-bold text-gray-400 uppercase tracking-wider mb-1">Nama Anda</label>
                                <input type="text" id="client-name" placeholder="cth: Ahmad" class="w-full bg-dark-900 border border-gray-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-500 transition-colors">
                            </div>

                            <div>
                                <label for="client-location" class="block text-xs font-bold text-gray-400 uppercase tracking-wider mb-1">Lokasi Anda</label>
                                <input type="text" id="client-location" placeholder="cth: Bangi, Selangor" class="w-full bg-dark-900 border border-gray-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-500 transition-colors">
                            </div>

                            <button onclick="sendQuickEstimate()" class="w-full bg-brand-500 hover:bg-brand-600 text-dark-900 font-bold py-3.5 rounded-xl flex items-center justify-center gap-2 shadow-lg transition-colors mt-6">
                                <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8"/></svg>
                                Hantar Anggaran Sebutharga
                            </button>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Seksyen Perkhidmatan -->
    <section id="perkhidmatan" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16 space-y-4">
                <span class="text-brand-600 font-bold tracking-widest uppercase text-sm">Apa Yang Kami Lakukan</span>
                <h2 class="text-3xl sm:text-4xl font-black text-dark-900">Perkhidmatan Utama Isa Wiring</h2>
                <div class="w-20 h-1 bg-brand-500 mx-auto rounded-full"></div>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Wiring -->
                <div class="bg-dark-50 p-8 rounded-3xl border border-gray-100 hover:border-brand-300 hover:shadow-xl hover:-translate-y-1 transition-all flex flex-col justify-between">
                    <div>
                        <div class="bg-brand-100 w-14 h-14 rounded-2xl flex items-center justify-center text-brand-700 mb-6 shadow-sm">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13 10V3L4 14h7v7l9-11h-7z"/></svg>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-dark-900">Wiring Elektrik</h3>
                        <p class="text-gray-600 text-sm leading-relaxed mb-6">Pendawaian baru 1/3 fasa, tukar DB Box, tambah soket, pasang lampu & kipas, baiki litar pintas.</p>
                    </div>
                    <a href="https://wa.me/60189141560" target="_blank" class="text-brand-600 hover:text-brand-700 font-bold text-sm inline-flex items-center gap-2 group">Tempah Wiring &rarr;</a>
                </div>

                <!-- Aircond -->
                <div class="bg-dark-50 p-8 rounded-3xl border border-gray-100 hover:border-brand-300 hover:shadow-xl hover:-translate-y-1 transition-all flex flex-col justify-between">
                    <div>
                        <div class="bg-brand-100 w-14 h-14 rounded-2xl flex items-center justify-center text-brand-700 mb-6 shadow-sm">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-dark-900">Servis Aircond</h3>
                        <p class="text-gray-600 text-sm leading-relaxed mb-6">Pemasangan unit baru, servis kimia, tambah gas, baiki kebocoran atau aircond tak sejuk.</p>
                    </div>
                    <a href="https://wa.me/60189141560" target="_blank" class="text-brand-600 hover:text-brand-700 font-bold text-sm inline-flex items-center gap-2 group">Tempah Aircond &rarr;</a>
                </div>

                <!-- Autogate -->
                <div class="bg-dark-50 p-8 rounded-3xl border border-gray-100 hover:border-brand-300 hover:shadow-xl hover:-translate-y-1 transition-all flex flex-col justify-between">
                    <div>
                        <div class="bg-brand-100 w-14 h-14 rounded-2xl flex items-center justify-center text-brand-700 mb-6 shadow-sm">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"/></svg>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-dark-900">Sistem Autogate</h3>
                        <p class="text-gray-600 text-sm leading-relaxed mb-6">Pasang sistem Swing/Fold/Sliding baru, tukar bateri, baiki remote & papan kawalan.</p>
                    </div>
                    <a href="https://wa.me/60189141560" target="_blank" class="text-brand-600 hover:text-brand-700 font-bold text-sm inline-flex items-center gap-2 group">Tempah Autogate &rarr;</a>
                </div>

                <!-- CCTV -->
                <div class="bg-dark-50 p-8 rounded-3xl border border-gray-100 hover:border-brand-300 hover:shadow-xl hover:-translate-y-1 transition-all flex flex-col justify-between">
                    <div>
                        <div class="bg-brand-100 w-14 h-14 rounded-2xl flex items-center justify-center text-brand-700 mb-6 shadow-sm">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z"/></svg>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-dark-900">Pasang CCTV</h3>
                        <p class="text-gray-600 text-sm leading-relaxed mb-6">Pemasangan kamera HD, pemantauan dari telefon bimbit, sistem amaran pintar & rakaman 24 jam.</p>
                    </div>
                    <a href="https://wa.me/60189141560" target="_blank" class="text-brand-600 hover:text-brand-700 font-bold text-sm inline-flex items-center gap-2 group">Tempah CCTV &rarr;</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Galeri Hasil Kerja (Slaid) -->
    <section id="hasil-kerja" class="py-20 bg-dark-900 text-white overflow-hidden relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between mb-12 gap-4">
                <div class="space-y-4">
                    <span class="text-brand-400 font-bold tracking-widest uppercase text-sm">Bukti Kualiti</span>
                    <h2 class="text-3xl sm:text-4xl font-black">Galeri Hasil Kerja Isa Wiring</h2>
                </div>
                <div class="flex gap-3">
                    <button id="prev-slide" class="w-12 h-12 rounded-xl border-2 border-gray-700 hover:border-brand-400 text-gray-400 hover:text-brand-400 flex items-center justify-center transition-all active:scale-95" aria-label="Slaid Kiri">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M15 19l-7-7 7-7"/></svg>
                    </button>
                    <button id="next-slide" class="w-12 h-12 rounded-xl border-2 border-gray-700 hover:border-brand-400 text-gray-400 hover:text-brand-400 flex items-center justify-center transition-all active:scale-95" aria-label="Slaid Kanan">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M9 5l7 7-7 7"/></svg>
                    </button>
                </div>
            </div>

            <div class="relative overflow-hidden rounded-3xl" id="slider-container">
                <div id="slider-track" class="flex transition-transform duration-500 ease-out cursor-grab active:cursor-grabbing">
                    
                    <!-- Slaid 1: Wiring -->
                    <div class="w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-2">
                        <div class="bg-dark-800 rounded-3xl overflow-hidden border border-gray-700/50 group h-full flex flex-col">
                            <div class="relative aspect-[4/3] bg-gray-950 overflow-hidden">
                                <img src="https://i.ibb.co/sdLBnWtX/image.jpg" 
                                     alt="Wiring Kerja" 
                                     class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105">
                                <div class="absolute top-4 left-4 bg-brand-500 text-dark-900 text-xs font-bold px-3 py-1 rounded-full uppercase">Wiring</div>
                            </div>
                            <div class="p-6 flex-grow flex flex-col justify-between">
                                <div>
                                    <h3 class="text-lg font-bold mb-2 uppercase group-hover:text-brand-400 transition-colors">Wiring</h3>
                                    <p class="text-sm text-gray-400">Kerja-kerja pengemasan dan pendawaian DB Box 3-fasa bagi memastikan keselamatan elektrikal rumah.</p>
                                </div>
                                <span class="text-xs text-brand-400 font-bold mt-4 uppercase tracking-wider">Projek: Rumah Kediaman</span>
                            </div>
                        </div>
                    </div>

                    <!-- Slaid 2: Aircond -->
                    <div class="w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-2">
                        <div class="bg-dark-800 rounded-3xl overflow-hidden border border-gray-700/50 group h-full flex flex-col">
                            <div class="relative aspect-[4/3] bg-gray-950 overflow-hidden">
                                <img src="https://i.ibb.co/206xh0Bz/image.jpg" 
                                     alt="Unit Aircond Midea" 
                                     class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105">
                                <div class="absolute top-4 left-4 bg-brand-500 text-dark-900 text-xs font-bold px-3 py-1 rounded-full uppercase">Aircond</div>
                            </div>
                            <div class="p-6 flex-grow flex flex-col justify-between">
                                <div>
                                    <h3 class="text-lg font-bold mb-2 uppercase group-hover:text-brand-400 transition-colors">AIRCOND</h3>
                                    <p class="text-sm text-gray-400">Membekal, Memasang, Membaiki & Servis unit pendingin hawa untuk keselesaan anda.</p>
                                </div>
                                <span class="text-xs text-brand-400 font-bold mt-4 uppercase tracking-wider">Projek: Kawasan Berdekatan</span>
                            </div>
                        </div>
                    </div>

                    <!-- Slaid 3: Autogate -->
                    <div class="w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-2">
                        <div class="bg-dark-800 rounded-3xl overflow-hidden border border-gray-700/50 group h-full flex flex-col">
                            <div class="relative aspect-[4/3] bg-gray-950 overflow-hidden">
                                <img src="https://i.ibb.co/23CWmqLm/image.jpg" 
                                     alt="Pemasangan Autogate" 
                                     class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105">
                                <div class="absolute top-4 left-4 bg-brand-500 text-dark-900 text-xs font-bold px-3 py-1 rounded-full uppercase">Autogate</div>
                            </div>
                            <div class="p-6 flex-grow flex flex-col justify-between">
                                <div>
                                    <h3 class="text-lg font-bold mb-2 uppercase group-hover:text-brand-400 transition-colors">autogate</h3>
                                    <p class="text-sm text-gray-400">Membekal, memasang, membaiki pelbagai jenis autogate.</p>
                                </div>
                                <span class="text-xs text-brand-400 font-bold mt-4 uppercase tracking-wider">Projek: KAWASAN BERDEKATAN</span>
                            </div>
                        </div>
                    </div>

                    <!-- Slaid 4: CCTV (BAHARU) -->
                    <div class="w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-2">
                        <div class="bg-dark-800 rounded-3xl overflow-hidden border border-gray-700/50 group h-full flex flex-col">
                            <div class="relative aspect-[4/3] bg-gray-950 overflow-hidden">
                                <img src="https://i.ibb.co/ZpL9CsPT/image.jpg" 
                                     alt="Sistem CCTV Hikvision" 
                                     class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105">
                                <div class="absolute top-4 left-4 bg-brand-500 text-dark-900 text-xs font-bold px-3 py-1 rounded-full uppercase">CCTV</div>
                            </div>
                            <div class="p-6 flex-grow flex flex-col justify-between">
                                <div>
                                    <h3 class="text-lg font-bold mb-2 uppercase group-hover:text-brand-400 transition-colors">cctv</h3>
                                    <p class="text-sm text-gray-400">Membekal dan memasang CCTV jenama Hikvision. Pelbagai pakej disediakan.</p>
                                </div>
                                <span class="text-xs text-brand-400 font-bold mt-4 uppercase tracking-wider">Projek: KAWASAN BERDEKATAN</span>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
            <div id="slider-dots" class="flex justify-center gap-2 mt-8"></div>
        </div>
    </section>

    <!-- Kenapa Pilih Kami -->
    <section class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div class="relative">
                    <div class="absolute inset-0 bg-brand-500/10 rounded-3xl transform rotate-3 scale-95 md:scale-100"></div>
                    <div class="relative bg-dark-900 text-white p-8 md:p-12 rounded-3xl border border-gray-100 shadow-xl overflow-hidden">
                        <div class="absolute -bottom-10 -right-10 w-40 h-40 bg-brand-500/20 rounded-full blur-2xl"></div>
                        <h3 class="text-2xl font-black mb-6 tracking-wide">Komitmen Kami</h3>
                        <div class="space-y-6">
                            <div class="flex gap-4">
                                <div class="bg-brand-500/20 text-brand-400 w-10 h-10 rounded-xl flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white text-base">Keselamatan Utama</h4>
                                    <p class="text-gray-400 text-sm">Pendawaian mengikut spesifikasi keselamatan bagi mengelakkan litar pintas.</p>
                                </div>
                            </div>
                            <div class="flex gap-4">
                                <div class="bg-brand-500/20 text-brand-400 w-10 h-10 rounded-xl flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white text-base">Menepati Masa</h4>
                                    <p class="text-gray-400 text-sm">Menghormati masa pelanggan adalah keutamaan perkhidmatan kami.</p>
                                </div>
                            </div>
                            <div class="flex gap-4">
                                <div class="bg-brand-500/20 text-brand-400 w-10 h-10 rounded-xl flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"/></svg>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white text-base">Harga Telus</h4>
                                    <p class="text-gray-400 text-sm">Sebut harga dipersetujui terlebih dahulu tanpa caj tersembunyi.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="space-y-6">
                    <span class="text-brand-600 font-bold tracking-widest uppercase text-sm">Kenapa Pilih Kami</span>
                    <h2 class="text-3xl sm:text-4xl font-black text-dark-900 leading-tight tracking-tight">Penyelesaian Elektrikal Kediaman Yang Dipercayai</h2>
                    <p class="text-gray-600">Kami adalah juruteknik elektrikal bertauliah tempatan yang berpengalaman luas dalam mengendalikan pelbagai kes kerosakan elektrik dan sistem mekanikal rumah.</p>
                    <div class="grid grid-cols-2 gap-6 pt-4">
                        <div class="bg-dark-50 p-5 rounded-2xl border border-gray-100">
                            <span class="block text-3xl font-black text-brand-600">200+</span>
                            <span class="text-sm font-bold text-dark-900 uppercase">Projek Selesai</span>
                        </div>
                        <div class="bg-dark-50 p-5 rounded-2xl border border-gray-100">
                            <span class="block text-3xl font-black text-brand-600">Pantas</span>
                            <span class="text-sm font-bold text-dark-900 uppercase tracking-tighter">Sedia Bertindak</span>
                        </div>
                    </div>
                    <div class="pt-4">
                        <a href="https://wa.me/60189141560" target="_blank" class="bg-dark-900 text-white hover:bg-black font-bold px-8 py-4 rounded-2xl inline-flex items-center gap-3 shadow-lg hover:scale-[1.02] active:scale-95 transition-all">
                            WhatsApp Sekarang
                            <svg class="w-5 h-5 text-brand-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M14 5l7 7m0 0l-7 7m7-7H3"/></svg>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Seruan Tindakan (Call to Action) -->
    <section class="bg-brand-500 py-16 text-dark-900">
        <div class="max-w-5xl mx-auto px-4 text-center space-y-6">
            <h2 class="text-3xl sm:text-4xl font-black tracking-tight leading-none uppercase">Ada Kecemasan Elektrik?</h2>
            <p class="text-lg text-dark-900/80 max-w-2xl mx-auto font-medium">Jangan biarkan kerosakan elektrik membahayakan keselamatan keluarga anda. Kami sedia membantu bila-bila masa sahaja.</p>
            <div class="pt-4">
                <a href="https://wa.me/60189141560" target="_blank" class="bg-dark-900 text-white hover:bg-black font-black px-10 py-5 rounded-2xl inline-flex items-center gap-3 shadow-2xl hover:scale-105 active:scale-95 transition-all text-lg">
                    HUBUNGI ISA: 018-9141560
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark-900 text-gray-400 py-12 border-t border-gray-800 text-center">
        <div class="max-w-7xl mx-auto px-4">
            <p class="text-white font-black text-xl mb-4 tracking-wider uppercase">ISA WIRING</p>
            <p class="text-sm mb-6 max-w-md mx-auto opacity-80 leading-relaxed">Pakar elektrikal bertauliah untuk pendawaian, servis aircond, autogate dan CCTV anda.</p>
            <div class="flex justify-center gap-6 mb-6 text-sm font-medium">
                <a href="#home" class="hover:text-brand-400 transition-colors uppercase tracking-widest">Laman Utama</a>
                <span class="text-gray-700">|</span>
                <a href="#hasil-kerja" class="hover:text-brand-400 transition-colors uppercase tracking-widest">Galeri Slaid</a>
            </div>
            <a href="https://wa.me/60189141560" class="text-brand-400 font-bold text-lg hover:underline">018-9141560</a>
            <p class="mt-8 text-[10px] opacity-40 tracking-widest uppercase">&copy; 2026 Isa Wiring. Hak Cipta Terpelihara.</p>
        </div>
    </footer>

    <!-- Butang WhatsApp Terapung -->
    <a href="https://wa.me/60189141560" target="_blank" class="fixed bottom-6 right-6 z-50 bg-[#25D366] text-white p-4 rounded-full shadow-2xl hover:scale-110 active:scale-95 transition-all animate-bounce" style="animation-duration: 2.5s;" aria-label="WhatsApp Kami">
        <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397.01 12.008.01c3.202.001 6.212 1.246 8.477 3.513 2.266 2.268 3.507 5.28 3.505 8.484-.004 6.657-5.34 11.997-11.953 11.997-2.005-.001-3.973-.502-5.724-1.457L0 24zm6.59-4.846c1.6.95 3.188 1.449 4.825 1.451 5.436 0 9.86-4.37 9.864-9.799.002-2.63-1.023-5.101-2.885-6.963C16.588 1.981 14.115.957 11.5.957c-5.442 0-9.87 4.372-9.874 9.802-.001 1.774.502 3.509 1.457 5.032l-1.012 3.702 3.813-1.002z"/></svg>
    </a>

    <script>
        // Menu Mobil Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuBtn.addEventListener('click', () => mobileMenu.classList.toggle('hidden'));

        // Logik Sebut Harga WhatsApp
        const selectedServices = new Set();
        function toggleService(id) {
            const btn = document.getElementById(`btn-${id}`);
            if (selectedServices.has(id)) {
                selectedServices.delete(id);
                btn.className = btn.className.replace('border-brand-500 bg-brand-500/10 text-white', 'border-gray-700 bg-dark-900 text-gray-300');
            } else {
                selectedServices.add(id);
                btn.className = btn.className.replace('border-gray-700 bg-dark-900 text-gray-300', 'border-brand-500 bg-brand-500/10 text-white');
            }
        }

        function sendQuickEstimate() {
            const name = document.getElementById('client-name').value || 'Pelanggan';
            const loc = document.getElementById('client-location').value || 'Tidak dinyatakan';
            if (selectedServices.size === 0) return alert('Sila pilih sekurang-kurangnya satu perkhidmatan!');
            const text = encodeURIComponent(`Halo Isa Wiring!\n\nNama: ${name}\nLokasi: ${loc}\nServis Diperlukan: ${Array.from(selectedServices).join(', ')}`);
            window.open(`https://wa.me/60189141560?text=${text}`, '_blank');
        }

        // Logik Slider Galeri
        const track = document.getElementById('slider-track');
        const dotsContainer = document.getElementById('slider-dots');
        const slides = Array.from(track.children);
        let currentIndex = 0;

        function getItemsPerView() {
            if (window.innerWidth >= 1024) return 3; // lg
            if (window.innerWidth >= 768) return 2;  // md
            return 1;                                // sm
        }

        function updateSlider() {
            const width = slides[0].getBoundingClientRect().width;
            track.style.transform = `translateX(-${currentIndex * width}px)`;
            generateDots();
        }

        function generateDots() {
            dotsContainer.innerHTML = '';
            const count = slides.length - getItemsPerView() + 1;
            if (count < 1) return; // Tiada titik jika semua gambar muat dlm satu view
            
            for (let i = 0; i < count; i++) {
                const dot = document.createElement('button');
                dot.className = `w-3 h-3 rounded-full transition-all ${i === currentIndex ? 'bg-brand-500 w-6' : 'bg-gray-700'}`;
                dot.onclick = () => { currentIndex = i; updateSlider(); };
                dotsContainer.appendChild(dot);
            }
        }

        document.getElementById('next-slide').onclick = () => {
            if (currentIndex < slides.length - getItemsPerView()) { currentIndex++; updateSlider(); }
        };
        document.getElementById('prev-slide').onclick = () => {
            if (currentIndex > 0) { currentIndex--; updateSlider(); }
        };

        window.onresize = updateSlider;
        updateSlider();
    </script>
</body>
</html>html
<!DOCTYPE html>
<html lang="ms" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Isa Wiring - Pakar Pendawaian, Aircond, Autogate & CCTV</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#fffbeb',
                            100: '#fef3c7',
                            200: '#fde68a',
                            300: '#fcd34d',
                            400: '#fbbf24',
                            500: '#f59e0b', /* Warna utama kuning elektrik */
                            600: '#d97706',
                            700: '#b45309',
                            800: '#92400e',
                            900: '#78350f',
                        },
                        dark: {
                            50: '#f8fafc',
                            100: '#f1f5f9',
                            800: '#1e293b',
                            900: '#0f172a',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Kesan transisi lancar */
        .transition-all {
            transition: all 0.3s ease-in-out;
        }
        /* Bar skrol tersuai untuk rupa premium */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #1e293b;
        }
        ::-webkit-scrollbar-thumb {
            background: #fbbf24;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #d97706;
        }
    </style>
</head>
<body class="bg-dark-50 text-dark-900 font-sans antialiased selection:bg-brand-400 selection:text-dark-900">

    <!-- Bar Informasi Atas -->
    <div class="bg-dark-900 text-white py-2 px-4 text-xs md:text-sm border-b border-brand-500/20">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-2">
            <div class="flex items-center gap-4">
                <span class="flex items-center gap-1">
                    <svg class="w-4 h-4 text-brand-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"/><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
                    Kawasan Perkhidmatan: Selangor, Kuala Lumpur & Negeri Sembilan
                </span>
            </div>
            <div class="flex items-center gap-4">
                <span class="flex items-center gap-1">
                    <svg class="w-4 h-4 text-brand-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                    Isnin - Ahad (8:00 AM - 10:00 PM)
                </span>
            </div>
        </div>
    </div>

    <!-- Kepala Laman (Header Navigation) -->
    <header class="sticky top-0 z-50 bg-white/95 backdrop-blur-md shadow-md transition-all">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                
                <!-- Logo & Nama Brand bersebelahan -->
                <a href="#home" class="flex items-center gap-3 group">
                    <div class="bg-dark-900 p-2.5 rounded-xl border border-brand-400 shadow-inner group-hover:scale-105 transition-transform">
                        <!-- Logo Kilat SVG Tersuai -->
                        <svg class="w-8 h-8 text-brand-400 animate-pulse" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
                            <polygon points="13 2 3 14 12 14 11 22 21 10 12 10 13 2"></polygon>
                        </svg>
                    </div>
                    <div class="flex flex-col">
                        <span class="text-2xl font-black tracking-wider text-dark-900 uppercase">
                            Isa <span class="text-brand-500">Wiring</span>
                        </span>
                        <span class="text-[10px] tracking-widest text-gray-500 uppercase font-bold -mt-1">Pakar Elektrikal Anda</span>
                    </div>
                </a>

                <!-- Menu Desktop -->
                <nav class="hidden md:flex items-center gap-8 font-semibold text-gray-700">
                    <a href="#home" class="hover:text-brand-600 transition-colors">Utama</a>
                    <a href="#perkhidmatan" class="hover:text-brand-600 transition-colors">Perkhidmatan</a>
                    <a href="#hasil-kerja" class="hover:text-brand-600 transition-colors">Hasil Kerja</a>
                    <a href="https://wa.me/60189141560" target="_blank" class="bg-brand-500 hover:bg-brand-600 text-dark-900 px-5 py-2.5 rounded-xl flex items-center gap-2 shadow-lg hover:shadow-brand-500/20 active:scale-95 transition-all">
                        <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397.01 12.008.01c3.202.001 6.212 1.246 8.477 3.513 2.266 2.268 3.507 5.28 3.505 8.484-.004 6.657-5.34 11.997-11.953 11.997-2.005-.001-3.973-.502-5.724-1.457L0 24zm6.59-4.846c1.6.95 3.188 1.449 4.825 1.451 5.436 0 9.86-4.37 9.864-9.799.002-2.63-1.023-5.101-2.885-6.963C16.588 1.981 14.115.957 11.5.957c-5.442 0-9.87 4.372-9.874 9.802-.001 1.774.502 3.509 1.457 5.032l-1.012 3.702 3.813-1.002z"/></svg>
                        Hubungi Kami
                    </a>
                </nav>

                <!-- Butang Menu Mobil -->
                <button id="mobile-menu-btn" class="md:hidden p-2 rounded-lg text-gray-700 hover:bg-gray-100 focus:outline-none" aria-label="Toggle Menu">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"/></svg>
                </button>
            </div>
        </div>

        <!-- Menu Mobil -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100 px-4 py-4 space-y-3 shadow-lg">
            <a href="#home" class="block py-2 px-3 rounded-lg hover:bg-brand-50 text-gray-800 font-medium">Utama</a>
            <a href="#perkhidmatan" class="block py-2 px-3 rounded-lg hover:bg-brand-50 text-gray-800 font-medium">Perkhidmatan</a>
            <a href="#hasil-kerja" class="block py-2 px-3 rounded-lg hover:bg-brand-50 text-gray-800 font-medium">Hasil Kerja</a>
            <a href="https://wa.me/60189141560" target="_blank" class="w-full bg-brand-500 text-dark-900 py-3 rounded-xl flex items-center justify-center gap-2 font-bold shadow-md">
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397.01 12.008.01c3.202.001 6.212 1.246 8.477 3.513 2.266 2.268 3.507 5.28 3.505 8.484-.004 6.657-5.34 11.997-11.953 11.997-2.005-.001-3.973-.502-5.724-1.457L0 24zm6.59-4.846c1.6.95 3.188 1.449 4.825 1.451 5.436 0 9.86-4.37 9.864-9.799.002-2.63-1.023-5.101-2.885-6.963C16.588 1.981 14.115.957 11.5.957c-5.442 0-9.87 4.372-9.874 9.802-.001 1.774.502 3.509 1.457 5.032l-1.012 3.702 3.813-1.002z"/></svg>
                Hubungi Sekarang
            </a>
        </div>
    </header>

    <!-- Seksyen Hero -->
    <section id="home" class="relative bg-dark-900 text-white overflow-hidden py-20 lg:py-32">
        <div class="absolute inset-0 opacity-10 bg-[radial-gradient(#fbbf24_1px,transparent_1px)] [background-size:16px_16px]"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                    <span class="inline-flex items-center gap-2 bg-brand-500/10 text-brand-400 px-4 py-2 rounded-full text-sm font-semibold border border-brand-500/20">
                        <span class="w-2 h-2 rounded-full bg-brand-400 animate-ping"></span>
                        Servis Pantas & Profesional
                    </span>
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-black tracking-tight leading-none">
                        Selesaikan Masalah Elektrikal Rumah Anda Dengan <span class="text-brand-400">Selamat</span>
                    </h1>
                    <p class="text-gray-300 text-lg md:text-xl max-w-2xl mx-auto lg:mx-0">
                        Kami menyediakan khidmat pakar untuk **Pendawaian (Wiring)**, pemasangan **Aircond**, pemasangan sistem **Autogate**, dan pemasangan kamera **CCTV** berdefinisi tinggi.
                    </p>
                    
                    <div class="flex flex-col sm:flex-row gap-4 justify-center lg:justify-start">
                        <a href="https://wa.me/60189141560?text=Salam%20Isa%20Wiring.%20Saya%20nak%20tanya%20mengenai%20servis%20anda." target="_blank" class="bg-brand-500 hover:bg-brand-600 text-dark-900 font-bold px-8 py-4 rounded-2xl flex items-center justify-center gap-3 shadow-xl shadow-brand-500/10 hover:shadow-brand-500/20 hover:scale-[1.02] active:scale-95 transition-all text-lg">
                            <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397.01 12.008.01c3.202.001 6.212 1.246 8.477 3.513 2.266 2.268 3.507 5.28 3.505 8.484-.004 6.657-5.34 11.997-11.953 11.997-2.005-.001-3.973-.502-5.724-1.457L0 24zm6.59-4.846c1.6.95 3.188 1.449 4.825 1.451 5.436 0 9.86-4.37 9.864-9.799.002-2.63-1.023-5.101-2.885-6.963C16.588 1.981 14.115.957 11.5.957c-5.442 0-9.87 4.372-9.874 9.802-.001 1.774.502 3.509 1.457 5.032l-1.012 3.702 3.813-1.002z"/></svg>
                            Hubungi Melalui WhatsApp
                        </a>
                        <a href="#perkhidmatan" class="border-2 border-gray-600 hover:border-brand-400 hover:text-brand-400 font-bold px-8 py-4 rounded-2xl flex items-center justify-center transition-colors text-lg">
                            Lihat Perkhidmatan
                        </a>
                    </div>
                </div>

                <!-- Widget Anggaran Pintar -->
                <div class="lg:col-span-5">
                    <div class="bg-dark-800 rounded-3xl p-6 sm:p-8 border border-gray-700 shadow-2xl relative">
                        <div class="absolute -top-3 -right-3 bg-brand-500 text-dark-900 text-xs font-black px-3 py-1 rounded-full uppercase tracking-wider shadow">
                            Sebut Harga Percuma
                        </div>
                        <h3 class="text-xl font-bold text-white mb-4">Dapatkan Anggaran Pantas</h3>
                        <p class="text-gray-400 text-sm mb-6">Pilih perkhidmatan yang diperlukan & hantar terus ke telefon kami.</p>
                        
                        <div class="space-y-4">
                            <div>
                                <label class="block text-xs font-bold text-gray-400 uppercase tracking-wider mb-2">Pilih Perkhidmatan</label>
                                <div class="grid grid-cols-2 gap-2">
                                    <button onclick="toggleService('Wiring')" id="btn-Wiring" class="service-selector-btn py-2.5 px-3 rounded-xl border border-gray-700 text-sm font-semibold bg-dark-900 hover:border-brand-500 text-gray-300 hover:text-white flex items-center gap-2 transition-all">
                                        <span class="w-2.5 h-2.5 rounded-full bg-gray-600 status-dot"></span> Wiring
                                    </button>
                                    <button onclick="toggleService('Aircond')" id="btn-Aircond" class="service-selector-btn py-2.5 px-3 rounded-xl border border-gray-700 text-sm font-semibold bg-dark-900 hover:border-brand-500 text-gray-300 hover:text-white flex items-center gap-2 transition-all">
                                        <span class="w-2.5 h-2.5 rounded-full bg-gray-600 status-dot"></span> Aircond
                                    </button>
                                    <button onclick="toggleService('Autogate')" id="btn-Autogate" class="service-selector-btn py-2.5 px-3 rounded-xl border border-gray-700 text-sm font-semibold bg-dark-900 hover:border-brand-500 text-gray-300 hover:text-white flex items-center gap-2 transition-all">
                                        <span class="w-2.5 h-2.5 rounded-full bg-gray-600 status-dot"></span> Autogate
                                    </button>
                                    <button onclick="toggleService('CCTV')" id="btn-CCTV" class="service-selector-btn py-2.5 px-3 rounded-xl border border-gray-700 text-sm font-semibold bg-dark-900 hover:border-brand-500 text-gray-300 hover:text-white flex items-center gap-2 transition-all">
                                        <span class="w-2.5 h-2.5 rounded-full bg-gray-600 status-dot"></span> CCTV
                                    </button>
                                </div>
                            </div>

                            <div>
                                <label for="client-name" class="block text-xs font-bold text-gray-400 uppercase tracking-wider mb-1">Nama Anda</label>
                                <input type="text" id="client-name" placeholder="cth: Ahmad" class="w-full bg-dark-900 border border-gray-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-500 transition-colors">
                            </div>

                            <div>
                                <label for="client-location" class="block text-xs font-bold text-gray-400 uppercase tracking-wider mb-1">Lokasi Anda</label>
                                <input type="text" id="client-location" placeholder="cth: Bangi, Selangor" class="w-full bg-dark-900 border border-gray-700 rounded-xl px-4 py-3 text-white text-sm focus:outline-none focus:border-brand-500 transition-colors">
                            </div>

                            <button onclick="sendQuickEstimate()" class="w-full bg-brand-500 hover:bg-brand-600 text-dark-900 font-bold py-3.5 rounded-xl flex items-center justify-center gap-2 shadow-lg transition-colors mt-6">
                                <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8"/></svg>
                                Hantar Anggaran Sebutharga
                            </button>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Seksyen Perkhidmatan -->
    <section id="perkhidmatan" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16 space-y-4">
                <span class="text-brand-600 font-bold tracking-widest uppercase text-sm">Apa Yang Kami Lakukan</span>
                <h2 class="text-3xl sm:text-4xl font-black text-dark-900">Perkhidmatan Utama Isa Wiring</h2>
                <div class="w-20 h-1 bg-brand-500 mx-auto rounded-full"></div>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Wiring -->
                <div class="bg-dark-50 p-8 rounded-3xl border border-gray-100 hover:border-brand-300 hover:shadow-xl hover:-translate-y-1 transition-all flex flex-col justify-between">
                    <div>
                        <div class="bg-brand-100 w-14 h-14 rounded-2xl flex items-center justify-center text-brand-700 mb-6 shadow-sm">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13 10V3L4 14h7v7l9-11h-7z"/></svg>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-dark-900">Wiring Elektrik</h3>
                        <p class="text-gray-600 text-sm leading-relaxed mb-6">Pendawaian baru 1/3 fasa, tukar DB Box, tambah soket, pasang lampu & kipas, baiki litar pintas.</p>
                    </div>
                    <a href="https://wa.me/60189141560" target="_blank" class="text-brand-600 hover:text-brand-700 font-bold text-sm inline-flex items-center gap-2 group">Tempah Wiring &rarr;</a>
                </div>

                <!-- Aircond -->
                <div class="bg-dark-50 p-8 rounded-3xl border border-gray-100 hover:border-brand-300 hover:shadow-xl hover:-translate-y-1 transition-all flex flex-col justify-between">
                    <div>
                        <div class="bg-brand-100 w-14 h-14 rounded-2xl flex items-center justify-center text-brand-700 mb-6 shadow-sm">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-dark-900">Servis Aircond</h3>
                        <p class="text-gray-600 text-sm leading-relaxed mb-6">Pemasangan unit baru, servis kimia, tambah gas, baiki kebocoran atau aircond tak sejuk.</p>
                    </div>
                    <a href="https://wa.me/60189141560" target="_blank" class="text-brand-600 hover:text-brand-700 font-bold text-sm inline-flex items-center gap-2 group">Tempah Aircond &rarr;</a>
                </div>

                <!-- Autogate -->
                <div class="bg-dark-50 p-8 rounded-3xl border border-gray-100 hover:border-brand-300 hover:shadow-xl hover:-translate-y-1 transition-all flex flex-col justify-between">
                    <div>
                        <div class="bg-brand-100 w-14 h-14 rounded-2xl flex items-center justify-center text-brand-700 mb-6 shadow-sm">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"/></svg>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-dark-900">Sistem Autogate</h3>
                        <p class="text-gray-600 text-sm leading-relaxed mb-6">Pasang sistem Swing/Fold/Sliding baru, tukar bateri, baiki remote & papan kawalan.</p>
                    </div>
                    <a href="https://wa.me/60189141560" target="_blank" class="text-brand-600 hover:text-brand-700 font-bold text-sm inline-flex items-center gap-2 group">Tempah Autogate &rarr;</a>
                </div>

                <!-- CCTV -->
                <div class="bg-dark-50 p-8 rounded-3xl border border-gray-100 hover:border-brand-300 hover:shadow-xl hover:-translate-y-1 transition-all flex flex-col justify-between">
                    <div>
                        <div class="bg-brand-100 w-14 h-14 rounded-2xl flex items-center justify-center text-brand-700 mb-6 shadow-sm">
                            <svg class="w-8 h-8" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"/><path stroke-linecap="round" stroke-linejoin="round" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z"/></svg>
                        </div>
                        <h3 class="text-xl font-bold mb-3 text-dark-900">Pasang CCTV</h3>
                        <p class="text-gray-600 text-sm leading-relaxed mb-6">Pemasangan kamera HD, pemantauan dari telefon bimbit, sistem amaran pintar & rakaman 24 jam.</p>
                    </div>
                    <a href="https://wa.me/60189141560" target="_blank" class="text-brand-600 hover:text-brand-700 font-bold text-sm inline-flex items-center gap-2 group">Tempah CCTV &rarr;</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Galeri Hasil Kerja (Slaid) -->
    <section id="hasil-kerja" class="py-20 bg-dark-900 text-white overflow-hidden relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between mb-12 gap-4">
                <div class="space-y-4">
                    <span class="text-brand-400 font-bold tracking-widest uppercase text-sm">Bukti Kualiti</span>
                    <h2 class="text-3xl sm:text-4xl font-black">Galeri Hasil Kerja Isa Wiring</h2>
                </div>
                <div class="flex gap-3">
                    <button id="prev-slide" class="w-12 h-12 rounded-xl border-2 border-gray-700 hover:border-brand-400 text-gray-400 hover:text-brand-400 flex items-center justify-center transition-all active:scale-95" aria-label="Slaid Kiri">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M15 19l-7-7 7-7"/></svg>
                    </button>
                    <button id="next-slide" class="w-12 h-12 rounded-xl border-2 border-gray-700 hover:border-brand-400 text-gray-400 hover:text-brand-400 flex items-center justify-center transition-all active:scale-95" aria-label="Slaid Kanan">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M9 5l7 7-7 7"/></svg>
                    </button>
                </div>
            </div>

            <div class="relative overflow-hidden rounded-3xl" id="slider-container">
                <div id="slider-track" class="flex transition-transform duration-500 ease-out cursor-grab active:cursor-grabbing">
                    
                    <!-- Slaid 1: Wiring -->
                    <div class="w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-2">
                        <div class="bg-dark-800 rounded-3xl overflow-hidden border border-gray-700/50 group h-full flex flex-col">
                            <div class="relative aspect-[4/3] bg-gray-950 overflow-hidden">
                                <img src="https://i.ibb.co/sdLBnWtX/image.jpg" 
                                     alt="Wiring Kerja" 
                                     class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105">
                                <div class="absolute top-4 left-4 bg-brand-500 text-dark-900 text-xs font-bold px-3 py-1 rounded-full uppercase">Wiring</div>
                            </div>
                            <div class="p-6 flex-grow flex flex-col justify-between">
                                <div>
                                    <h3 class="text-lg font-bold mb-2 uppercase group-hover:text-brand-400 transition-colors">Wiring</h3>
                                    <p class="text-sm text-gray-400">Kerja-kerja pengemasan dan pendawaian DB Box 3-fasa bagi memastikan keselamatan elektrikal rumah.</p>
                                </div>
                                <span class="text-xs text-brand-400 font-bold mt-4 uppercase tracking-wider">Projek: Rumah Kediaman</span>
                            </div>
                        </div>
                    </div>

                    <!-- Slaid 2: Aircond -->
                    <div class="w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-2">
                        <div class="bg-dark-800 rounded-3xl overflow-hidden border border-gray-700/50 group h-full flex flex-col">
                            <div class="relative aspect-[4/3] bg-gray-950 overflow-hidden">
                                <img src="https://i.ibb.co/206xh0Bz/image.jpg" 
                                     alt="Unit Aircond Midea" 
                                     class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105">
                                <div class="absolute top-4 left-4 bg-brand-500 text-dark-900 text-xs font-bold px-3 py-1 rounded-full uppercase">Aircond</div>
                            </div>
                            <div class="p-6 flex-grow flex flex-col justify-between">
                                <div>
                                    <h3 class="text-lg font-bold mb-2 uppercase group-hover:text-brand-400 transition-colors">AIRCOND</h3>
                                    <p class="text-sm text-gray-400">Membekal, Memasang, Membaiki & Servis unit pendingin hawa untuk keselesaan anda.</p>
                                </div>
                                <span class="text-xs text-brand-400 font-bold mt-4 uppercase tracking-wider">Projek: Kawasan Berdekatan</span>
                            </div>
                        </div>
                    </div>

                    <!-- Slaid 3: Autogate -->
                    <div class="w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-2">
                        <div class="bg-dark-800 rounded-3xl overflow-hidden border border-gray-700/50 group h-full flex flex-col">
                            <div class="relative aspect-[4/3] bg-gray-950 overflow-hidden">
                                <img src="https://i.ibb.co/23CWmqLm/image.jpg" 
                                     alt="Pemasangan Autogate" 
                                     class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105">
                                <div class="absolute top-4 left-4 bg-brand-500 text-dark-900 text-xs font-bold px-3 py-1 rounded-full uppercase">Autogate</div>
                            </div>
                            <div class="p-6 flex-grow flex flex-col justify-between">
                                <div>
                                    <h3 class="text-lg font-bold mb-2 uppercase group-hover:text-brand-400 transition-colors">autogate</h3>
                                    <p class="text-sm text-gray-400">Membekal, memasang, membaiki pelbagai jenis autogate.</p>
                                </div>
                                <span class="text-xs text-brand-400 font-bold mt-4 uppercase tracking-wider">Projek: KAWASAN BERDEKATAN</span>
                            </div>
                        </div>
                    </div>

                    <!-- Slaid 4: CCTV (BAHARU) -->
                    <div class="w-full md:w-1/2 lg:w-1/3 flex-shrink-0 px-2">
                        <div class="bg-dark-800 rounded-3xl overflow-hidden border border-gray-700/50 group h-full flex flex-col">
                            <div class="relative aspect-[4/3] bg-gray-950 overflow-hidden">
                                <img src="https://i.ibb.co/ZpL9CsPT/image.jpg" 
                                     alt="Sistem CCTV Hikvision" 
                                     class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105">
                                <div class="absolute top-4 left-4 bg-brand-500 text-dark-900 text-xs font-bold px-3 py-1 rounded-full uppercase">CCTV</div>
                            </div>
                            <div class="p-6 flex-grow flex flex-col justify-between">
                                <div>
                                    <h3 class="text-lg font-bold mb-2 uppercase group-hover:text-brand-400 transition-colors">cctv</h3>
                                    <p class="text-sm text-gray-400">Membekal dan memasang CCTV jenama Hikvision. Pelbagai pakej disediakan.</p>
                                </div>
                                <span class="text-xs text-brand-400 font-bold mt-4 uppercase tracking-wider">Projek: KAWASAN BERDEKATAN</span>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
            <div id="slider-dots" class="flex justify-center gap-2 mt-8"></div>
        </div>
    </section>

    <!-- Kenapa Pilih Kami -->
    <section class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div class="relative">
                    <div class="absolute inset-0 bg-brand-500/10 rounded-3xl transform rotate-3 scale-95 md:scale-100"></div>
                    <div class="relative bg-dark-900 text-white p-8 md:p-12 rounded-3xl border border-gray-100 shadow-xl overflow-hidden">
                        <div class="absolute -bottom-10 -right-10 w-40 h-40 bg-brand-500/20 rounded-full blur-2xl"></div>
                        <h3 class="text-2xl font-black mb-6 tracking-wide">Komitmen Kami</h3>
                        <div class="space-y-6">
                            <div class="flex gap-4">
                                <div class="bg-brand-500/20 text-brand-400 w-10 h-10 rounded-xl flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white text-base">Keselamatan Utama</h4>
                                    <p class="text-gray-400 text-sm">Pendawaian mengikut spesifikasi keselamatan bagi mengelakkan litar pintas.</p>
                                </div>
                            </div>
                            <div class="flex gap-4">
                                <div class="bg-brand-500/20 text-brand-400 w-10 h-10 rounded-xl flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white text-base">Menepati Masa</h4>
                                    <p class="text-gray-400 text-sm">Menghormati masa pelanggan adalah keutamaan perkhidmatan kami.</p>
                                </div>
                            </div>
                            <div class="flex gap-4">
                                <div class="bg-brand-500/20 text-brand-400 w-10 h-10 rounded-xl flex items-center justify-center shrink-0">
                                    <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"/></svg>
                                </div>
                                <div>
                                    <h4 class="font-bold text-white text-base">Harga Telus</h4>
                                    <p class="text-gray-400 text-sm">Sebut harga dipersetujui terlebih dahulu tanpa caj tersembunyi.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="space-y-6">
                    <span class="text-brand-600 font-bold tracking-widest uppercase text-sm">Kenapa Pilih Kami</span>
                    <h2 class="text-3xl sm:text-4xl font-black text-dark-900 leading-tight tracking-tight">Penyelesaian Elektrikal Kediaman Yang Dipercayai</h2>
                    <p class="text-gray-600">Kami adalah juruteknik elektrikal bertauliah tempatan yang berpengalaman luas dalam mengendalikan pelbagai kes kerosakan elektrik dan sistem mekanikal rumah.</p>
                    <div class="grid grid-cols-2 gap-6 pt-4">
                        <div class="bg-dark-50 p-5 rounded-2xl border border-gray-100">
                            <span class="block text-3xl font-black text-brand-600">200+</span>
                            <span class="text-sm font-bold text-dark-900 uppercase">Projek Selesai</span>
                        </div>
                        <div class="bg-dark-50 p-5 rounded-2xl border border-gray-100">
                            <span class="block text-3xl font-black text-brand-600">Pantas</span>
                            <span class="text-sm font-bold text-dark-900 uppercase tracking-tighter">Sedia Bertindak</span>
                        </div>
                    </div>
                    <div class="pt-4">
                        <a href="https://wa.me/60189141560" target="_blank" class="bg-dark-900 text-white hover:bg-black font-bold px-8 py-4 rounded-2xl inline-flex items-center gap-3 shadow-lg hover:scale-[1.02] active:scale-95 transition-all">
                            WhatsApp Sekarang
                            <svg class="w-5 h-5 text-brand-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M14 5l7 7m0 0l-7 7m7-7H3"/></svg>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Seruan Tindakan (Call to Action) -->
    <section class="bg-brand-500 py-16 text-dark-900">
        <div class="max-w-5xl mx-auto px-4 text-center space-y-6">
            <h2 class="text-3xl sm:text-4xl font-black tracking-tight leading-none uppercase">Ada Kecemasan Elektrik?</h2>
            <p class="text-lg text-dark-900/80 max-w-2xl mx-auto font-medium">Jangan biarkan kerosakan elektrik membahayakan keselamatan keluarga anda. Kami sedia membantu bila-bila masa sahaja.</p>
            <div class="pt-4">
                <a href="https://wa.me/60189141560" target="_blank" class="bg-dark-900 text-white hover:bg-black font-black px-10 py-5 rounded-2xl inline-flex items-center gap-3 shadow-2xl hover:scale-105 active:scale-95 transition-all text-lg">
                    HUBUNGI ISA: 018-9141560
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark-900 text-gray-400 py-12 border-t border-gray-800 text-center">
        <div class="max-w-7xl mx-auto px-4">
            <p class="text-white font-black text-xl mb-4 tracking-wider uppercase">ISA WIRING</p>
            <p class="text-sm mb-6 max-w-md mx-auto opacity-80 leading-relaxed">Pakar elektrikal bertauliah untuk pendawaian, servis aircond, autogate dan CCTV anda.</p>
            <div class="flex justify-center gap-6 mb-6 text-sm font-medium">
                <a href="#home" class="hover:text-brand-400 transition-colors uppercase tracking-widest">Laman Utama</a>
                <span class="text-gray-700">|</span>
                <a href="#hasil-kerja" class="hover:text-brand-400 transition-colors uppercase tracking-widest">Galeri Slaid</a>
            </div>
            <a href="https://wa.me/60189141560" class="text-brand-400 font-bold text-lg hover:underline">018-9141560</a>
            <p class="mt-8 text-[10px] opacity-40 tracking-widest uppercase">&copy; 2026 Isa Wiring. Hak Cipta Terpelihara.</p>
        </div>
    </footer>

    <!-- Butang WhatsApp Terapung -->
    <a href="https://wa.me/60189141560" target="_blank" class="fixed bottom-6 right-6 z-50 bg-[#25D366] text-white p-4 rounded-full shadow-2xl hover:scale-110 active:scale-95 transition-all animate-bounce" style="animation-duration: 2.5s;" aria-label="WhatsApp Kami">
        <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946C.06 5.348 5.397.01 12.008.01c3.202.001 6.212 1.246 8.477 3.513 2.266 2.268 3.507 5.28 3.505 8.484-.004 6.657-5.34 11.997-11.953 11.997-2.005-.001-3.973-.502-5.724-1.457L0 24zm6.59-4.846c1.6.95 3.188 1.449 4.825 1.451 5.436 0 9.86-4.37 9.864-9.799.002-2.63-1.023-5.101-2.885-6.963C16.588 1.981 14.115.957 11.5.957c-5.442 0-9.87 4.372-9.874 9.802-.001 1.774.502 3.509 1.457 5.032l-1.012 3.702 3.813-1.002z"/></svg>
    </a>

    <script>
        // Menu Mobil Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        mobileMenuBtn.addEventListener('click', () => mobileMenu.classList.toggle('hidden'));

        // Logik Sebut Harga WhatsApp
        const selectedServices = new Set();
        function toggleService(id) {
            const btn = document.getElementById(`btn-${id}`);
            if (selectedServices.has(id)) {
                selectedServices.delete(id);
                btn.className = btn.className.replace('border-brand-500 bg-brand-500/10 text-white', 'border-gray-700 bg-dark-900 text-gray-300');
            } else {
                selectedServices.add(id);
                btn.className = btn.className.replace('border-gray-700 bg-dark-900 text-gray-300', 'border-brand-500 bg-brand-500/10 text-white');
            }
        }

        function sendQuickEstimate() {
            const name = document.getElementById('client-name').value || 'Pelanggan';
            const loc = document.getElementById('client-location').value || 'Tidak dinyatakan';
            if (selectedServices.size === 0) return alert('Sila pilih sekurang-kurangnya satu perkhidmatan!');
            const text = encodeURIComponent(`Halo Isa Wiring!\n\nNama: ${name}\nLokasi: ${loc}\nServis Diperlukan: ${Array.from(selectedServices).join(', ')}`);
            window.open(`https://wa.me/60189141560?text=${text}`, '_blank');
        }

        // Logik Slider Galeri
        const track = document.getElementById('slider-track');
        const dotsContainer = document.getElementById('slider-dots');
        const slides = Array.from(track.children);
        let currentIndex = 0;

        function getItemsPerView() {
            if (window.innerWidth >= 1024) return 3; // lg
            if (window.innerWidth >= 768) return 2;  // md
            return 1;                                // sm
        }

        function updateSlider() {
            const width = slides[0].getBoundingClientRect().width;
            track.style.transform = `translateX(-${currentIndex * width}px)`;
            generateDots();
        }

        function generateDots() {
            dotsContainer.innerHTML = '';
            const count = slides.length - getItemsPerView() + 1;
            if (count < 1) return; // Tiada titik jika semua gambar muat dlm satu view
            
            for (let i = 0; i < count; i++) {
                const dot = document.createElement('button');
                dot.className = `w-3 h-3 rounded-full transition-all ${i === currentIndex ? 'bg-brand-500 w-6' : 'bg-gray-700'}`;
                dot.onclick = () => { currentIndex = i; updateSlider(); };
                dotsContainer.appendChild(dot);
            }
        }

        document.getElementById('next-slide').onclick = () => {
            if (currentIndex < slides.length - getItemsPerView()) { currentIndex++; updateSlider(); }
        };
        document.getElementById('prev-slide').onclick = () => {
            if (currentIndex > 0) { currentIndex--; updateSlider(); }
        };

        window.onresize = updateSlider;
        updateSlider();
    </script>
</body>
</html>
