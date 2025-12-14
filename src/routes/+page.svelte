<script lang="ts">
	import { onMount } from 'svelte';

    // Insurance carriers and partners
    const partners = [
        { name: 'Tryg', src: 'https://placehold.co/80x30?text=Tryg' },
        { name: 'If', src: 'https://placehold.co/80x30?text=If' },
        { name: 'Gjensidige', src: 'https://placehold.co/80x30?text=Gjensidige' },
        { name: 'Protector', src: 'https://placehold.co/80x30?text=Protector' },
        { name: 'Frende', src: 'https://placehold.co/80x30?text=Frende' },
        { name: 'Eika', src: 'https://placehold.co/80x30?text=Eika' },
        { name: 'SpareBank 1', src: 'https://placehold.co/80x30?text=SpareBank1' },
        { name: 'Storebrand', src: 'https://placehold.co/80x30?text=Storebrand' },
    ];

    const articles = [
        {
            tag: 'Case Study',
            title: 'From 3 hours to 3 minutes',
            desc: 'How a Norwegian brokerage reduced policy processing time by 100x with Effara\'s AI agents',
            img: 'https://placehold.co/300x200/E8E8E3/1a1a1a?text=Case+Study',
            bg: 'bg-primary-50'
        },
        {
            tag: 'Product',
            title: 'Pre-built carrier integrations',
            desc: 'Effara connects directly to major insurance carriers, eliminating manual data entry and integration headaches',
            img: 'https://placehold.co/300x200/D4C5A3/1a1a1a?text=Integrations',
            bg: 'bg-gray-50'
        },
        {
            tag: 'Industry',
            title: 'The future of insurance brokerage',
            desc: 'How AI agents are transforming the way small brokerages compete with larger firms',
            img: 'https://placehold.co/300x200/E8E8E3/1a1a1a?text=Future',
            bg: 'bg-primary-50'
        },
        {
            tag: 'Guide',
            title: 'Say goodbye to Excel workflows',
            desc: 'A practical guide to automating your brokerage operations without changing your existing processes',
            img: 'https://placehold.co/300x200/F0E6D2/1a1a1a?text=Guide',
            bg: 'bg-gray-50'
        }
    ];

    const testimonials = [
        {
            quote: "Effara transformed our brokerage. What used to take hours now takes minutes. We can finally focus on our clients instead of paperwork.",
            author: "Lars Andersen",
            role: "Managing Director",
            company: "Nordic Insurance Brokers",
            img: "/generated/image-professional-insurance-broker-smiling-co-1765713119710-1.webp"
        }
    ];
</script>

<div class="min-h-screen bg-white text-gray-900 font-sans selection:bg-gray-200">
    <!-- Header -->
    <header class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-sm">
        <div class="max-w-[1600px] mx-auto px-6 py-6 flex justify-between items-center">
            <div>
                <a href="/" class="text-2xl font-semibold tracking-tight">
                    Effara
                </a>
            </div>
            <div>
                <a href="#" class="bg-black text-white px-5 py-2.5 text-xs font-medium rounded-sm hover:bg-gray-800 transition-colors">
                    Get Started
                </a>
            </div>
        </div>
    </header>

    <main class="pt-32 pb-20">
        <div class="max-w-[1600px] mx-auto px-6 grid grid-cols-12 gap-8">
            <!-- Sidebar Navigation -->
            <div class="col-span-2 hidden lg:block sticky top-32 h-fit">
                <nav class="flex flex-col space-y-3 text-xs text-gray-500 font-medium">
                    <a href="#" class="text-black">Home</a>
                    <a href="#" class="hover:text-black transition-colors">Product</a>
                    <a href="#" class="hover:text-black transition-colors">Integrations</a>
                    <a href="#" class="hover:text-black transition-colors">Resources</a>
                    <a href="#" class="hover:text-black transition-colors">Team</a>
                </nav>
            </div>

            <!-- Main Content Area -->
            <div class="col-span-12 lg:col-span-10 space-y-32">
                
                <!-- Hero Section -->
                <section class="relative">
                    <div class="relative w-full h-[600px] overflow-hidden rounded-sm">
                        <!-- Hero Background Image -->
                        <img src="/generated/image-insurance-broker-working-at-desk-with-co-1765713116643-0.webp" alt="Insurance broker at work" class="absolute inset-0 w-full h-full object-cover" />
                        
                        <div class="absolute inset-0 bg-gradient-to-r from-black/60 to-black/20"></div>
                        
                        <div class="absolute inset-0 flex flex-col items-center justify-center p-12 text-center">
                            <h1 class="text-4xl md:text-5xl font-normal text-white mb-6 max-w-3xl leading-tight">
                                Automate insurance brokerage workflows with AI agents
                            </h1>
                            <p class="text-lg text-white/90 mb-12 max-w-2xl">
                                Complete tasks 100x faster. From manual Excel work to automated policy processing in minutes.
                            </p>

                            <!-- Logos Card -->
                            <div class="bg-white/95 backdrop-blur-sm p-8 rounded-sm shadow-sm max-w-3xl w-full">
                                <p class="text-[10px] text-gray-500 mb-6 uppercase tracking-wide">
                                    Trusted by brokerages and integrated with leading insurance carriers
                                </p>
                                <div class="grid grid-cols-4 md:grid-cols-4 gap-8 items-center justify-items-center opacity-80 grayscale">
                                    {#each partners as partner}
                                        <div class="h-6 flex items-center justify-center">
                                            <span class="text-[10px] font-bold text-gray-800">{partner.name}</span>
                                        </div>
                                    {/each}
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- How Effara Works Section -->
                <section>
                    <div class="flex justify-between items-baseline mb-24 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900 max-w-xl leading-tight">
                            How Effara transforms broker workflows
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Our solution</span>
                    </div>

                    <div class="relative min-h-[800px]">
                        <!-- Diagram (Sticky/Fixed positioning simulation) -->
                        <div class="absolute right-0 top-0 w-1/2 p-8 bg-gray-50 rounded-sm">
                            <div class="text-[10px] text-gray-500 mb-4">Automated workflow in action</div>
                            <div class="flex items-center justify-between gap-4">
                                <div class="w-32 h-32 bg-black text-white flex flex-col items-center justify-center p-4 rounded-sm">
                                    <div class="mb-2">
                                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                                    </div>
                                    <span class="text-[10px] uppercase tracking-wider text-center">Email & Excel</span>
                                </div>
                                
                                <div class="flex-1 h-32 bg-primary-100/50 border border-primary-200 rounded-sm flex flex-col items-center justify-center relative">
                                    <span class="text-[10px] text-gray-500 uppercase absolute top-2 left-4">AI Agents</span>
                                    <div class="w-full border-t border-dashed border-gray-300 absolute top-1/2"></div>
                                    
                                    <!-- AI Agent Icon -->
                                    <div class="absolute -bottom-6 bg-white border border-primary-300 p-2 shadow-sm rounded-sm flex items-center gap-2">
                                        <div class="w-8 h-10 border border-primary-400 flex items-center justify-center bg-primary-50">
                                            <svg class="w-4 h-4 text-primary-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                                        </div>
                                        <div class="text-[8px] leading-tight text-gray-500">
                                            100x<br>FASTER
                                        </div>
                                    </div>
                                </div>

                                <div class="w-32 h-32 bg-gradient-to-br from-primary-700 to-primary-600 text-white flex flex-col items-center justify-center p-4 rounded-sm">
                                    <div class="mb-2">
                                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
                                    </div>
                                    <span class="text-[10px] uppercase tracking-wider text-center">Policy Ready</span>
                                </div>
                            </div>
                        </div>

                        <!-- Text Blocks -->
                        <div class="absolute left-0 top-[200px] max-w-xs">
                            <div class="flex gap-4">
                                <span class="bg-black text-white w-5 h-5 flex items-center justify-center text-xs font-medium shrink-0 rounded-sm">1</span>
                                <p class="text-sm text-gray-600 leading-relaxed">
                                    AI agents automatically process emails, extract policy data from Excel files, and communicate with insurance carriers.
                                </p>
                            </div>
                        </div>

                        <div class="absolute left-0 top-[400px] max-w-xs">
                            <div class="flex gap-4">
                                <span class="bg-black text-white w-5 h-5 flex items-center justify-center text-xs font-medium shrink-0 rounded-sm">2</span>
                                <p class="text-sm text-gray-600 leading-relaxed">
                                    Pre-built integrations with major carriers eliminate manual data entry and reduce errors by 95%.
                                </p>
                            </div>
                        </div>

                        <div class="absolute left-0 top-[600px] max-w-xs">
                            <div class="flex gap-4">
                                <span class="bg-black text-white w-5 h-5 flex items-center justify-center text-xs font-medium shrink-0 rounded-sm">3</span>
                                <p class="text-sm text-gray-600 leading-relaxed">
                                    What took hours now takes minutes. Brokers can focus on clients instead of paperwork.
                                </p>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- About Effara Section -->
                <section>
                    <div class="flex justify-between items-baseline mb-16 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900">
                            Built by insurance experts for insurance brokers
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">About Effara</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-3 gap-12 text-sm leading-relaxed text-gray-600 mb-24">
                        <div class="space-y-6">
                            <p>
                                Effara is transforming insurance brokerage with agentic AI. We automate the tedious workflows that consume hours of broker time every day.
                            </p>
                            <p>
                                Starting with Norwegian SME brokerages, we're building the tools that help small brokers compete with larger firms through intelligent automation.
                            </p>
                        </div>
                        <div class="space-y-6">
                            <p>
                                Our founders—Terje, Paal, and Magnus—bring deep insurance industry experience combined with digital innovation expertise. They've seen firsthand how brokers waste time on manual Excel work and email processing when they should be focusing on clients.
                            </p>
                            <p>
                                We built proprietary AI agents specifically for insurance workflows. These agents understand policy data, carrier requirements, and brokerage operations. They work alongside brokers, handling the repetitive tasks while humans focus on relationships and strategic decisions.
                            </p>
                        </div>
                        <div class="space-y-6">
                            <p>
                                Our pre-built carrier integrations eliminate the biggest barrier to automation: integration complexity. Brokers can start automating immediately without technical headaches.
                            </p>
                            <p>
                                With 600,000 insurance brokers globally and growing demand for efficiency, we're scaling from Norwegian SMEs to become the automation platform for brokerages worldwide. Our goal: 6,000 licenses and 100x faster workflows for every broker.
                            </p>
                        </div>
                    </div>

                    <!-- Team Image -->
                    <div class="bg-gray-50 rounded-sm overflow-hidden">
                        <img src="/generated/image-team-of-insurance-professionals-collabor-1765713121889-2.webp" alt="Effara team" class="w-full h-[400px] object-cover" />
                    </div>
                </section>

                <!-- Key Features Dark Section -->
                <section class="bg-gray-950 text-white rounded-sm overflow-hidden relative min-h-[400px] flex items-center">
                    <!-- Background Graphic -->
                    <div class="absolute inset-0 opacity-20">
                        <div class="absolute bottom-0 left-0 right-0 h-64 bg-gradient-to-t from-primary-900/30 to-transparent"></div>
                         <!-- Abstract network/connection lines -->
                        <svg class="absolute bottom-0 w-full h-full text-primary-900/20" viewBox="0 0 100 100" preserveAspectRatio="none">
                            <path d="M0 100 Q 50 50 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                            <path d="M0 100 Q 50 40 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                            <path d="M0 100 Q 50 30 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                        </svg>
                    </div>

                    <div class="relative z-10 p-16 w-full grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                        <div>
                            <h2 class="text-3xl font-light mb-6">
                                Pre-built carrier integrations<br>that just work
                            </h2>
                            <p class="text-sm text-gray-400 mb-8 max-w-md">
                                Connect instantly to major Norwegian and European insurance carriers. No technical setup, no integration headaches. Start automating on day one.
                            </p>
                            <button class="bg-white text-black px-6 py-2 text-xs font-medium rounded-sm hover:bg-gray-200 transition-colors">
                                View Integrations
                            </button>
                        </div>
                        <div class="flex justify-end">
                            <div class="grid grid-cols-2 gap-4">
                                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-sm p-6 flex flex-col items-center justify-center text-center">
                                    <svg class="w-8 h-8 mb-3 text-primary-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                                    <div class="text-2xl font-bold mb-1">100x</div>
                                    <div class="text-[10px] text-gray-400 uppercase">Faster</div>
                                </div>
                                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-sm p-6 flex flex-col items-center justify-center text-center">
                                    <svg class="w-8 h-8 mb-3 text-primary-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
                                    <div class="text-2xl font-bold mb-1">95%</div>
                                    <div class="text-[10px] text-gray-400 uppercase">Less Errors</div>
                                </div>
                                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-sm p-6 flex flex-col items-center justify-center text-center">
                                    <svg class="w-8 h-8 mb-3 text-primary-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"></path></svg>
                                    <div class="text-2xl font-bold mb-1">24/7</div>
                                    <div class="text-[10px] text-gray-400 uppercase">Automation</div>
                                </div>
                                <div class="bg-white/5 backdrop-blur-sm border border-white/10 rounded-sm p-6 flex flex-col items-center justify-center text-center">
                                    <svg class="w-8 h-8 mb-3 text-primary-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z"></path></svg>
                                    <div class="text-2xl font-bold mb-1">6k</div>
                                    <div class="text-[10px] text-gray-400 uppercase">Target Users</div>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- Testimonials -->
                <section>
                    <div class="flex justify-between items-baseline mb-16 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900">
                            Trusted by insurance brokers
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Testimonials</span>
                    </div>

                    <div class="relative">
                        <div class="flex gap-8 overflow-hidden">
                            <div class="w-full md:w-[800px] shrink-0 bg-gray-50 flex">
                                <div class="w-1/3 shrink-0">
                                    <img src="/generated/image-professional-insurance-broker-smiling-co-1765713119710-1.webp" alt="Lars Andersen" class="w-full h-full object-cover" />
                                </div>
                                <div class="w-2/3 p-12 flex flex-col justify-center">
                                    <blockquote class="text-xl font-light leading-relaxed mb-8">
                                        "Effara transformed our brokerage. What used to take hours now takes minutes. We can finally focus on our clients instead of paperwork."
                                    </blockquote>
                                    <div class="flex items-center gap-2 mb-2">
                                        <div class="w-4 h-4 bg-primary-500 rounded-full"></div>
                                        <span class="text-xs font-semibold text-gray-500">Nordic Insurance Brokers</span>
                                    </div>
                                    <div>
                                        <div class="font-medium">Lars Andersen</div>
                                        <div class="text-xs text-gray-500">Managing Director</div>
                                    </div>
                                </div>
                            </div>
                            <!-- Next slide preview -->
                            <div class="w-1/3 shrink-0 opacity-50 bg-gray-100 flex items-center justify-center">
                                <div class="text-center p-8">
                                    <div class="text-4xl mb-4">⚡</div>
                                    <div class="text-sm text-gray-500">More testimonials coming soon</div>
                                </div>
                            </div>
                        </div>
                        
                        <!-- Navigation Button -->
                        <button class="absolute top-0 right-0 -mt-12 w-8 h-8 bg-black text-white flex items-center justify-center hover:bg-gray-800">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg>
                        </button>
                    </div>
                </section>

                <!-- Read More / Articles -->
                <section>
                    <div class="flex justify-between items-baseline mb-16 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900">
                            Read more
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Articles</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                        {#each articles as article}
                            <div class="group cursor-pointer">
                                <div class="relative aspect-square mb-6 overflow-hidden {article.bg} flex items-center justify-center">
                                    <span class="absolute top-4 left-4 text-[10px] uppercase tracking-wider bg-white/50 px-2 py-1 backdrop-blur-sm">{article.tag}</span>
                                    <!-- Use text overlay instead of image if image fails, but styling div with bg color -->
                                    <div class="text-center p-4">
                                        <!-- Placeholder graphic -->
                                        <div class="text-2xl font-serif italic opacity-50">{article.title.split(' ')[0]}</div>
                                    </div>
                                </div>
                                <h3 class="text-lg font-normal mb-3 leading-tight group-hover:underline decoration-1 underline-offset-4">
                                    {article.title}
                                </h3>
                                <p class="text-xs text-gray-500 mb-4 leading-relaxed">
                                    {article.desc}
                                </p>
                                <a href="#" class="text-xs font-medium underline decoration-1 underline-offset-4">Read more</a>
                            </div>
                        {/each}
                    </div>
                </section>

            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-white pt-32 pb-12 border-t border-gray-100 relative overflow-hidden">
        <!-- Large Background Watermark -->
        <div class="absolute left-0 bottom-0 text-[20vw] font-bold text-gray-50 leading-none select-none pointer-events-none -mb-12 -ml-12">
            Effara
        </div>

        <div class="max-w-[1600px] mx-auto px-6 relative z-10">
            <div class="flex flex-col md:flex-row justify-between items-end md:items-center mb-24">
                <div class="text-lg font-light">Automate with confidence</div>
                <div class="text-lg font-light underline decoration-1 underline-offset-4">EFFARA.COM</div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-12 gap-8 items-end">
                <div class="md:col-span-6">
                    <!-- Logo -->
                    <div class="flex items-center gap-4 mb-4">
                        <div class="w-8 h-8 rounded-full bg-primary-600 flex items-center justify-center">
                            <svg class="w-4 h-4 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                        </div>
                        <div class="text-xl font-semibold tracking-tight">
                            Effara
                        </div>
                    </div>
                    <p class="text-xs text-gray-500 max-w-xs">
                        Automating insurance brokerage workflows with agentic AI agents for 100x faster task completion.
                    </p>
                </div>
                
                <div class="md:col-span-6 flex flex-col md:flex-row justify-between items-end md:items-end gap-8">
                    <div class="text-[10px] text-gray-400">
                        © 2025 Effara
                    </div>
                    
                    <div class="flex gap-8 text-[10px] font-medium uppercase tracking-wide">
                        <div class="flex flex-col gap-2">
                            <a href="#" class="hover:text-primary-600 transition-colors">Team</a>
                            <a href="#" class="hover:text-primary-600 transition-colors">Product</a>
                            <a href="#" class="hover:text-primary-600 transition-colors">Contact</a>
                        </div>
                        <div class="flex flex-col gap-2">
                            <a href="#" class="hover:text-primary-600 transition-colors">Terms</a>
                            <a href="#" class="hover:text-primary-600 transition-colors">Privacy Policy</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</div>

<style>
    /* Custom scrollbar hide for clean look */
    ::-webkit-scrollbar {
        width: 0px;
        background: transparent;
    }
</style>

