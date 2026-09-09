<svelte:head>
	<title>Yuka Store — iPhone Baru & Second Original di Garut</title>
	<meta
		name="description"
		content="Yuka Store Shop & Service di Garut. Spesialis iPhone baru & second original, bergaransi, bisa tukar tambah."
	/>
</svelte:head>

<script lang="ts">
	const waNumber = '628973744455';
	const waDisplay = '0897-3744-455';
	const address = 'Jl. Raya Bayongbong Muara Sanding No. 111, Garut';
	const mapsLink = `https://www.google.com/maps/search/?api=1&query=${encodeURIComponent(address)}`;
	const igHandle = 'yukastore__';
	const tiktokHandle = 'yukastore__';
	const waLink = (pesan: string) => `https://wa.me/${waNumber}?text=${encodeURIComponent(pesan)}`;

	const lineup = [
		{
			tag: '01 / BARU',
			title: 'iPhone Baru',
			desc: 'Segel & garansi resmi. Aktivasi dibantu sampai iCloud jadi.',
			msg: 'Halo Yuka Store, iPhone baru apa saja yang ready hari ini?'
		},
		{
			tag: '02 / SECOND',
			title: 'iPhone Second',
			desc: 'Cek 21 titik. iCloud bersih, BH jujur, foto + video real.',
			msg: 'Halo Yuka Store, minta list iPhone second yang ready + harganya dong'
		},
		{
			tag: '03 / TRADE-IN',
			title: 'Tukar Tambah',
			desc: 'iPhone lamamu jadi diskon. Taksiran 20 menit via WA.',
			msg: 'Halo, saya mau tukar tambah. iPhone saya ... BH ... minus ...'
		}
	];

	const faqs = [
		{ q: 'Apakah iPhone second-nya original?', a: 'Ya. Cek fisik, fungsi, IMEI, iCloud. Unit bermasalah kami tolak.' },
		{ q: 'Kenapa tidak ada daftar harga?', a: 'Harga second fluktuatif harian. Chat WA untuk harga akurat hari ini.' },
		{ q: 'Bisa tukar tambah?', a: 'Bisa. Kirim tipe, kapasitas, BH, minus, dan kelengkapan via WA.' },
		{ q: 'Bisa COD / kirim luar kota?', a: 'Bisa COD sekitar Garut & kirim se-Indonesia + asuransi.' },
		{ q: 'Ada servis iPhone?', a: 'Ada. Ganti baterai, LCD, kamera — bergaransi.' }
	];
</script>

<!-- NAVBAR glass -->
<header class="fixed inset-x-0 top-0 z-50">
	<div class="mx-auto mt-2 flex h-14 max-w-6xl items-center justify-between px-3 md:mt-3 md:h-16 md:px-6">
		<div class="glass flex h-full w-full items-center justify-between gap-2 rounded-2xl px-3 shadow-2xl md:px-4">
			<a href="#top" class="flex min-w-0 items-center gap-2">
				<span class="flex shrink-0 items-center overflow-hidden rounded-xl bg-black px-2 py-1 ring-1 ring-white/20">
					<img src="/logo-navbar.jpeg" alt="Yuka Store" class="h-7 w-auto md:h-8" />
				</span>
				<span class="font-display hidden whitespace-nowrap text-lg font-extrabold tracking-tight sm:inline">Yuka Store</span>
			</a>
			<nav class="hidden items-center gap-7 text-sm font-medium text-white/70 lg:flex">
				<a href="#iphone" class="hover:text-white">iPhone</a>
				<a href="#kenapa" class="hover:text-white">Kenapa</a>
				<a href="#toko" class="hover:text-white">Toko</a>
				<a href="#faq" class="hover:text-white">FAQ</a>
			</nav>
			<a
				href={waLink('Halo Yuka Store, mau tanya stok iPhone dong')}
				target="_blank"
				class="shrink-0 whitespace-nowrap rounded-full bg-white px-4 py-2 text-[13px] font-bold text-black transition hover:scale-105 hover:bg-fuchsia-200 md:px-5 md:py-2.5 md:text-sm"
			>
				Chat WA ↗
			</a>
		</div>
	</div>
</header>

<main id="top" class="relative bg-[#08080c]">
	<!-- HERO ARTISTIK -->
	<section class="grain relative overflow-hidden pb-10 pt-32 md:pt-40">
		<!-- blob background -->
		<div class="animate-blob absolute -left-32 top-10 h-[420px] w-[420px] rounded-full bg-violet-600/40 blur-[120px]"></div>
		<div class="animate-blob absolute right-[-100px] top-64 h-[380px] w-[380px] rounded-full bg-cyan-400/25 blur-[120px]" style="animation-delay:-4s"></div>
		<div class="animate-blob absolute bottom-0 left-1/3 h-[300px] w-[500px] rounded-full bg-fuchsia-600/25 blur-[130px]" style="animation-delay:-8s"></div>

		<div class="relative mx-auto max-w-6xl px-4 md:px-6">
			<p class="inline-flex max-w-full flex-wrap items-center gap-2 rounded-full border border-white/15 bg-white/5 px-3 py-1.5 text-[10px] font-semibold tracking-[0.15em] text-white/70 md:px-4 md:text-xs md:tracking-[0.2em]">
				<span class="h-2 w-2 shrink-0 animate-pulse rounded-full bg-green-400"></span>
				<span class="break-words">GARUT • SHOP & SERVICE • FOKUS IPHONE</span>
			</p>

			<h1 class="font-display mt-6 text-[46px] font-black leading-[0.92] tracking-tight sm:text-6xl md:text-[96px] md:leading-[0.9]">
				<span class="block">YUKA</span>
				<span class="text-stroke block">STORE</span>
				<span class="text-gradient block">iPHONE LOVER.</span>
			</h1>

			<div class="mt-8 grid gap-6 md:grid-cols-[1.2fr_0.8fr] md:items-end">
				<p class="max-w-xl text-base leading-relaxed text-white/70 md:text-lg">
					Bukan toko HP biasa. Kami kurasi <strong class="text-white">iPhone baru & second original</strong>,
					cek 21 titik, garansi jelas, bisa tukar tambah. Harga? Update harian via WhatsApp — no jebakan.
				</p>
				<div class="flex flex-col gap-3 sm:flex-row sm:flex-wrap md:justify-end">
					<a
						href={waLink('Halo Yuka Store, mau tanya stok iPhone yang ready hari ini')}
						target="_blank"
						class="flex items-center justify-center gap-2.5 rounded-full bg-white py-2.5 pl-3 pr-7 font-bold text-black shadow-[0_10px_40px_rgba(255,255,255,0.3)] transition hover:scale-105"
					>
						<img src="/whatsapp-logo.png" alt="WA" class="h-9 w-9 shrink-0 rounded-full" />
						<span class="whitespace-nowrap">Tanya Stok Hari Ini</span>
					</a>
					<a
						href="#toko"
						class="glass rounded-full px-7 py-3.5 text-center font-bold text-white transition hover:scale-105"
					>
						Lihat Toko ↓
					</a>
				</div>
			</div>

			<!-- hero visual: di HP kartu TIDAK numpuk gambar, banner full terlihat -->
			<div class="relative mt-8 md:mt-12">
				<img
					src="/banner-toko.jpeg"
					alt="Yuka Store Shop & Service - iPhone Baru Second Original"
					class="h-auto w-full rounded-2xl border border-white/15 object-contain shadow-2xl md:rounded-[28px] md:object-cover"
				/>
				<!-- Mobile: kartu statis di bawah gambar -->
				<div class="mt-3 grid grid-cols-2 gap-2.5 md:hidden">
					<div class="glass min-w-0 rounded-2xl p-3">
						<p class="text-[10px] font-bold tracking-widest text-white/60">CEK 21 TITIK</p>
						<p class="font-display truncate text-[15px] font-extrabold">100% Original ✓</p>
					</div>
					<div class="glass min-w-0 rounded-2xl p-3">
						<p class="text-[10px] font-bold tracking-widest text-white/60">RATING</p>
						<p class="font-display truncate text-[15px] font-extrabold">4.9★ • 2rb+</p>
					</div>
				</div>
				<!-- Desktop: kartu melayang -->
				<div class="glass animate-float absolute left-8 top-8 hidden rounded-2xl p-4 md:block">
					<p class="text-xs font-bold tracking-widest text-white/60">CEK 21 TITIK</p>
					<p class="font-display text-xl font-extrabold">100% Original ✓</p>
				</div>
				<div class="glass animate-float absolute bottom-8 right-8 hidden rounded-2xl p-4 md:block" style="animation-delay:-3s">
					<p class="text-xs font-bold tracking-widest text-white/60">RATING</p>
					<p class="font-display text-xl font-extrabold">4.9★ • 2rb+ terjual</p>
				</div>
				<div class="animate-spin-slow absolute -top-10 right-10 hidden h-28 w-28 items-center justify-center rounded-full border border-dashed border-white/30 bg-black/40 text-center text-[10px] font-bold tracking-widest backdrop-blur lg:flex">
					SCROLL<br />↓<br />GARUT
				</div>
			</div>
		</div>

		<!-- marquee -->
		<div class="mt-12 overflow-hidden border-y border-white/10 bg-white/[0.03] py-4">
			<div class="animate-marquee flex w-max gap-8 whitespace-nowrap font-display text-2xl font-extrabold text-white/80">
				{#each Array(2) as _}
					<span>iPHONE BARU ✦ SECOND MULUS ✦ TUKAR TAMBAH ✦ SERVICE BERGARANSI ✦ AKSESORIS ORI ✦&nbsp;</span>
				{/each}
			</div>
		</div>
	</section>

	<!-- LINEUP BENTO -->
	<section id="iphone" class="relative mx-auto max-w-6xl px-4 py-20 md:px-6 md:py-28">
		<div class="flex flex-wrap items-end justify-between gap-4">
			<h2 class="font-display text-5xl font-black leading-none md:text-7xl">
				Pilih<br /><span class="text-white/40">jalanmu.</span>
			</h2>
			<p class="max-w-xs text-white/60">Tanpa katalog harga mati. Semua via chat — cepat & jujur.</p>
		</div>
		<div class="mt-10 grid gap-4 md:grid-cols-3">
			{#each lineup as item, i}
				<a
					href={waLink(item.msg)}
					target="_blank"
					class="apple-card group relative overflow-hidden rounded-[28px] border border-white/10 bg-gradient-to-b from-white/[0.1] to-white/[0.02] p-8"
				>
					<p class="text-xs font-bold tracking-[0.2em] text-fuchsia-300">{item.tag}</p>
					<h3 class="font-display mt-3 text-4xl font-extrabold">{item.title}</h3>
					<p class="mt-3 text-white/60">{item.desc}</p>
					<p class="mt-8 inline-flex items-center gap-2 rounded-full bg-white px-5 py-2.5 text-sm font-bold text-black transition group-hover:bg-fuchsia-200">
						Chat sekarang <span class="transition group-hover:translate-x-1">→</span>
					</p>
					<span class="font-display pointer-events-none absolute -bottom-6 -right-2 text-[120px] font-black text-white/[0.06]">0{i + 1}</span>
				</a>
			{/each}
		</div>
	</section>

	<!-- KENAPA: horizontal artistic -->
	<section id="kenapa" class="border-y border-white/10 bg-white/[0.02] py-20">
		<div class="mx-auto grid max-w-6xl gap-10 px-4 md:grid-cols-[0.9fr_1.1fr] md:px-6">
			<div>
				<img src="/logo-stacked-crop.jpeg" alt="logo" class="w-40 rounded-2xl border border-white/10" />
				<h2 class="font-display mt-6 text-5xl font-black leading-[0.95]">Kenapa<br />harus Yuka?</h2>
				<p class="mt-4 text-white/60">Vibe Apple, ketelitian teknisi, harga kaki lima yang jujur.</p>
				<a href={waLink('Halo, saya mau konsultasi iPhone')} target="_blank" class="apple-link mt-4 inline-block font-semibold">Konsultasi gratis &gt;</a>
			</div>
			<div class="grid gap-4 sm:grid-cols-2">
				<div class="glass rounded-3xl p-6"><p class="text-3xl">🔍</p><h3 class="mt-3 font-bold">Cek 21 titik</h3><p class="mt-1 text-sm text-white/60">Face ID, True Tone, BH, sinyal — semua dicek.</p></div>
				<div class="glass rounded-3xl p-6 md:translate-y-6"><p class="text-3xl">🧾</p><h3 class="mt-3 font-bold">Nota + garansi</h3><p class="mt-1 text-sm text-white/60">Jelas tertulis. Komplain? Balik aja.</p></div>
				<div class="glass rounded-3xl p-6"><p class="text-3xl">🔄</p><h3 class="mt-3 font-bold">Trade-in cepat</h3><p class="mt-1 text-sm text-white/60">20 menit taksiran via WA.</p></div>
				<div class="glass rounded-3xl p-6 md:translate-y-6"><p class="text-3xl">🛠️</p><h3 class="mt-3 font-bold">Service + sparepart</h3><p class="mt-1 text-sm text-white/60">Baterai, LCD, kamera bergaransi.</p></div>
			</div>
		</div>
	</section>

	<!-- TOKO -->
	<section id="toko" class="mx-auto max-w-6xl px-4 py-20 md:px-6 md:py-28">
		<h2 class="font-display text-center text-5xl font-black md:text-7xl">Mampir<span class="text-gradient"> & buktikan.</span></h2>
		<p class="mt-3 text-center text-white/60">{address} • {waDisplay}</p>
		<div class="mt-10 grid gap-4 md:grid-cols-2">
			<div class="group relative overflow-hidden rounded-[28px] border border-white/10">
				<img src="/toko.jpeg" alt="toko" class="h-64 w-full object-cover transition duration-700 group-hover:scale-105 sm:h-80 md:h-[420px]" />
				<div class="absolute inset-x-4 bottom-4 flex items-center justify-between rounded-2xl bg-black/60 p-4 backdrop-blur-xl">
					<p class="text-sm font-semibold">Etalase real • Coba sepuasnya</p>
					<a href={waLink('Halo, saya mau mampir ke toko')} target="_blank" class="rounded-full bg-white px-4 py-2 text-xs font-bold text-black">Sharelok →</a>
				</div>
			</div>
			<div class="overflow-hidden rounded-[28px] border border-white/10 bg-white/[0.04]">
				<iframe
					title="maps"
					src="https://www.google.com/maps?q={encodeURIComponent(address)}&output=embed"
					class="h-[320px] w-full border-0"
					loading="lazy"
					allowfullscreen
				></iframe>
				<div class="flex flex-wrap items-center justify-between gap-3 p-5">
					<p class="text-sm text-white/70">IG @{igHandle} • TikTok @{tiktokHandle}</p>
					<div class="flex gap-2">
						<a href="https://instagram.com/{igHandle}" target="_blank" class="rounded-full border border-white/20 px-4 py-2 text-xs font-bold hover:bg-white hover:text-black">IG</a>
						<a href="https://tiktok.com/@{tiktokHandle}" target="_blank" class="rounded-full border border-white/20 px-4 py-2 text-xs font-bold hover:bg-white hover:text-black">TikTok</a>
						<a href={mapsLink} target="_blank" class="rounded-full bg-white px-4 py-2 text-xs font-bold text-black">Rute</a>
					</div>
				</div>
			</div>
		</div>
	</section>

	<!-- FAQ -->
	<section id="faq" class="mx-auto max-w-3xl px-4 pb-24">
		<h2 class="font-display text-center text-4xl font-black">FAQ santai.</h2>
		<div class="mt-8 space-y-3">
			{#each faqs as f}
				<details class="glass group rounded-2xl p-5">
					<summary class="flex cursor-pointer list-none items-center justify-between font-bold">
						{f.q}
						<span class="flex h-8 w-8 items-center justify-center rounded-full bg-white text-lg text-black transition group-open:rotate-45">+</span>
					</summary>
					<p class="mt-3 text-sm leading-relaxed text-white/65">{f.a}</p>
				</details>
			{/each}
		</div>
		<div class="relative mt-10 overflow-hidden rounded-[28px] bg-gradient-to-br from-violet-600 via-fuchsia-500 to-cyan-400 p-[1.5px]">
			<div class="rounded-[27px] bg-[#0c0c12] p-8 text-center md:p-12">
				<h3 class="font-display text-4xl font-black">Galau pilih iPhone?</h3>
				<p class="mx-auto mt-3 max-w-md text-white/60">Sebut budget & kebutuhan. Kami balas 2–3 rekomendasi terbaik hari ini.</p>
				<a
					href={waLink('Halo Yuka Store, budget saya ... tolong rekomendasi dong')}
					target="_blank"
					class="mt-6 inline-flex items-center gap-2.5 rounded-full bg-white py-2.5 pl-3 pr-8 font-bold text-black transition hover:scale-105"
				>
					<img src="/whatsapp-logo.png" alt="WA" class="h-9 w-9 rounded-full" />
					Chat Sekarang — Fast Respon ⚡
				</a>
			</div>
		</div>
	</section>
</main>

<footer class="border-t border-white/10 bg-black/60 px-4 py-8 text-center text-xs text-white/45">
	<p class="font-display text-lg font-extrabold text-white">YUKA STORE® — SHOP & SERVICE</p>
	<p class="mt-2">{address} • WA {waDisplay} • IG/TikTok @{igHandle}</p>
	<p class="mt-1">© 2026 • Dibuat dengan ♥ di Garut</p>
</footer>

<a
	href={waLink('Halo Yuka Store!')}
	target="_blank"
	aria-label="Chat WhatsApp Yuka Store"
	class="fixed bottom-4 right-4 z-50 transition hover:scale-110 md:bottom-5 md:right-5"
>
	<img
		src="/whatsapp-logo.png"
		alt="Chat WhatsApp"
		class="h-12 w-12 rounded-full shadow-[0_10px_40px_rgba(37,211,102,0.5)] md:h-[60px] md:w-[60px]"
		width="60"
		height="60"
	/>
</a>
