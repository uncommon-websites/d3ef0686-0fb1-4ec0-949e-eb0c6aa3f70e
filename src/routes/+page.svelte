<script lang="ts">
	import { onMount } from 'svelte';

    // Placeholder data
    const partners = [
        { name: 'MITRE', src: 'https://placehold.co/80x30?text=MITRE' },
        { name: 'Stanford', src: 'https://placehold.co/80x30?text=Stanford' },
        { name: 'Google Cloud', src: 'https://placehold.co/80x30?text=Google' },
        { name: 'Newfront', src: 'https://placehold.co/80x30?text=Newfront' },
        { name: 'Cisco', src: 'https://placehold.co/80x30?text=Cisco' },
        { name: 'MongoDB', src: 'https://placehold.co/80x30?text=MongoDB' },
        { name: 'Orrick', src: 'https://placehold.co/80x30?text=Orrick' },
        { name: 'Cognition', src: 'https://placehold.co/80x30?text=Cognition' },
        { name: 'Ada', src: 'https://placehold.co/80x30?text=Ada' },
        { name: 'CoreWeave', src: 'https://placehold.co/80x30?text=CoreWeave' },
        { name: 'Alpharum', src: 'https://placehold.co/80x30?text=Alpharum' },
        { name: 'Virtue AI', src: 'https://placehold.co/80x30?text=Virtue' },
        { name: 'Hale Labs', src: 'https://placehold.co/80x30?text=Hale' },
        { name: 'Axiora', src: 'https://placehold.co/80x30?text=Axiora' },
        { name: 'Faculty', src: 'https://placehold.co/80x30?text=Faculty' },
        { name: 'Gray Swan', src: 'https://placehold.co/80x30?text=GraySwan' },
        { name: 'Witness AI', src: 'https://placehold.co/80x30?text=Witness' },
        { name: 'Newfront', src: 'https://placehold.co/80x30?text=Newfront' },
        { name: 'Carnegie Mellon', src: 'https://placehold.co/80x30?text=CMU' },
        { name: 'Fin', src: 'https://placehold.co/80x30?text=Fin' },
        { name: 'UiPath', src: 'https://placehold.co/80x30?text=UiPath' },
    ];

    const articles = [
        {
            tag: 'Article',
            title: 'Case study: How Intercom built',
            desc: 'Intercom achieved AIUC-1 certification of their AI agent, Fin',
            img: 'https://placehold.co/300x200/E8E8E3/1a1a1a?text=Fin',
            bg: 'bg-[#E8E8E3]'
        },
        {
            tag: 'Research',
            title: 'AI-Proofing The Board and C-suite',
            desc: 'Dr. Keri Pearlson at MIT Sloan and Rajiv Dattani at AIUC have written a new paper.',
            img: 'https://placehold.co/300x200/D4C5A3/1a1a1a?text=AI-proofing',
            bg: 'bg-[#D4C5A3]'
        },
        {
            tag: 'Research',
            title: 'Stanford Trustworthy AI Research x AIUC',
            desc: 'Stanford Professor Dr. Sanmi Koyejo on real-world AI risk for enterprises',
            img: 'https://placehold.co/300x200/E8E8E3/1a1a1a?text=Stanford',
            bg: 'bg-[#E8E8E3]'
        },
        {
            tag: 'Research',
            title: 'Orrick x AIUC partner on AIUC-1',
            desc: 'AIUC and top AI law firm Orrick, Herrington & Sutcliffe have partnered to create AIUC-1.',
            img: 'https://placehold.co/300x200/F0E6D2/1a1a1a?text=Orrick',
            bg: 'bg-[#F0E6D2]'
        }
    ];

    const testimonials = [
        {
            quote: "We need a SOC 2 for AI agents - a familiar, actionable standard for security and trust.",
            author: "Phil Venables",
            role: "Former CISO",
            company: "Google Cloud",
            img: "https://placehold.co/400x500/gray/white?text=Phil"
        }
    ];
</script>

<div class="min-h-screen bg-white text-gray-900 font-sans selection:bg-gray-200">
    <!-- Header -->
    <header class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-sm">
        <div class="max-w-[1600px] mx-auto px-6 py-6 flex justify-between items-start">
            <div class="w-64">
                <a href="/" class="text-sm font-medium leading-tight block max-w-[160px]">
                    Artificial Intelligence<br>Underwriting Company
                </a>
            </div>
            <div>
                <a href="#" class="bg-black text-white px-5 py-2.5 text-xs font-medium rounded-sm hover:bg-gray-800 transition-colors">
                    Request a Demo
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
                    <a href="#" class="hover:text-black transition-colors">AIUC-1</a>
                    <a href="#" class="hover:text-black transition-colors">Research</a>
                    <a href="#" class="hover:text-black transition-colors">Team</a>
                </nav>
            </div>

            <!-- Main Content Area -->
            <div class="col-span-12 lg:col-span-10 space-y-32">
                
                <!-- Hero Section -->
                <section class="relative">
                    <div class="relative w-full h-[600px] overflow-hidden rounded-sm">
                        <!-- Mountain Background Placeholder -->
                        <img src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?q=80&w=2000&auto=format&fit=crop" alt="Snowy mountains" class="absolute inset-0 w-full h-full object-cover" />
                        
                        <div class="absolute inset-0 flex flex-col items-center justify-center p-12 text-center">
                            <h1 class="text-4xl md:text-5xl font-normal text-gray-900 mb-12 max-w-2xl leading-tight">
                                Certify and insure AI agents<br>to unlock enterprise adoption
                            </h1>

                            <!-- Logos Card -->
                            <div class="bg-white/95 backdrop-blur-sm p-8 rounded-sm shadow-sm max-w-4xl w-full">
                                <p class="text-[10px] text-gray-500 mb-6 uppercase tracking-wide">
                                    Customers, partners & technical contributors securing AI progress with standards, audits, and insurance.
                                </p>
                                <div class="grid grid-cols-4 md:grid-cols-7 gap-8 items-center justify-items-center opacity-80 grayscale">
                                    {#each partners as partner}
                                        <div class="h-6 flex items-center justify-center">
                                            <!-- Using text as placeholder for logos to keep it clean if images fail, but trying to use the src -->
                                            <span class="text-[10px] font-bold text-gray-800">{partner.name}</span>
                                        </div>
                                    {/each}
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- How AIUC Unlocks Section -->
                <section>
                    <div class="flex justify-between items-baseline mb-24 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900 max-w-xl leading-tight">
                            How AIUC unlocks secure AI adoption for enterprises
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Our solution</span>
                    </div>

                    <div class="relative min-h-[800px]">
                        <!-- Diagram (Sticky/Fixed positioning simulation) -->
                        <div class="absolute right-0 top-0 w-1/2 p-8 bg-gray-50 rounded-sm">
                            <div class="text-[10px] text-gray-500 mb-4">3 - And insures their customers against</div>
                            <div class="flex items-center justify-between gap-4">
                                <div class="w-32 h-32 bg-black text-white flex flex-col items-center justify-center p-4 rounded-sm">
                                    <div class="mb-2">
                                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"></path></svg>
                                    </div>
                                    <span class="text-[10px] uppercase tracking-wider">AI Company</span>
                                </div>
                                
                                <div class="flex-1 h-32 bg-blue-100/50 border border-blue-200 rounded-sm flex flex-col items-center justify-center relative">
                                    <span class="text-[10px] text-gray-500 uppercase absolute top-2 left-4">Insurance</span>
                                    <div class="w-full border-t border-dashed border-gray-300 absolute top-1/2"></div>
                                    
                                    <!-- Certificate Icon -->
                                    <div class="absolute -bottom-6 bg-white border border-gray-200 p-2 shadow-sm rounded-sm flex items-center gap-2">
                                        <div class="w-8 h-10 border border-gray-300 flex items-center justify-center bg-gray-50">
                                            <div class="w-4 h-4 rounded-full border border-gray-400"></div>
                                        </div>
                                        <div class="text-[8px] leading-tight text-gray-500">
                                            AIUC-1<br>CERTIFICATION
                                        </div>
                                    </div>
                                </div>

                                <div class="w-32 h-32 bg-gradient-to-br from-blue-900 to-blue-700 text-white flex flex-col items-center justify-center p-4 rounded-sm">
                                    <div class="mb-2">
                                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"></path></svg>
                                    </div>
                                    <span class="text-[10px] uppercase tracking-wider">Enterprise</span>
                                </div>
                            </div>
                        </div>

                        <!-- Text Blocks -->
                        <div class="absolute left-0 top-[400px] max-w-xs">
                            <div class="flex gap-4">
                                <span class="bg-black text-white w-5 h-5 flex items-center justify-center text-xs font-medium shrink-0 rounded-sm">1</span>
                                <p class="text-sm text-gray-600 leading-relaxed">
                                    AI companies buy insurance to fully protect their enterprise customers in case an AI agent failure leads to business loss.
                                </p>
                            </div>
                        </div>

                        <div class="absolute left-0 top-[600px] max-w-xs">
                            <div class="flex gap-4">
                                <span class="bg-black text-white w-5 h-5 flex items-center justify-center text-xs font-medium shrink-0 rounded-sm">2</span>
                                <p class="text-sm text-gray-600 leading-relaxed">
                                    Certificates and insurance create the "confidence infrastructure" enterprises need to adopt.
                                </p>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- Confidence Infrastructure Section -->
                <section>
                    <div class="flex justify-between items-baseline mb-16 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900">
                            Confidence infrastructure for AI
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Insurance Built the Modern World</span>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-3 gap-12 text-sm leading-relaxed text-gray-600 mb-24">
                        <p>
                            We are an AI agent standards & insurance company based in San Francisco.
                        </p>
                        <div class="space-y-6">
                            <p>
                                We built the modern world with American ingenuity, free markets, and the courage to act in the face of uncertainty. Railroads, capital markets, the internet and the built world flourished after people and institutions bet money on their safety.
                            </p>
                            <p>
                                The most powerful technology in human history is reshaping our world. Every day, companies are racing to deploy AI. Enterprise leaders see the inevitable transformation. But they hesitate on one question: "How do we know this is secure?"
                            </p>
                        </div>
                        <div class="space-y-6">
                            <p>
                                Legal teams fear liability. Security leaders face novel attack vectors. Procurement teams can't compare providers. Over 1,000 AI-related bills have been introduced in U.S. state legislatures in 2025 alone. Decisions stall amid bureaucratic gridlock, while the technology advances at breakneck pace.
                            </p>
                            <p>
                                We are building the infrastructure to accelerate AI adoption by certifying and insuring AI agents. Insurance built the modern world once. It must do so again.
                            </p>
                        </div>
                    </div>

                    <!-- Featured In -->
                    <div class="bg-gray-50 rounded-sm p-8 flex items-center justify-between">
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider mr-8">Featured in :</span>
                        <div class="flex-1 flex justify-between items-center opacity-60 grayscale">
                            <span class="font-serif text-xl font-bold">The New York Times</span>
                            <span class="font-sans text-xl font-bold">NBC</span>
                            <span class="font-serif text-lg">Reinsurance News</span>
                            <span class="font-serif text-lg">FINANCIAL TIMES</span>
                            <span class="font-serif text-lg">FORTUNE</span>
                        </div>
                    </div>
                </section>

                <!-- AIUC-1 Dark Section -->
                <section class="bg-[#050A18] text-white rounded-sm overflow-hidden relative min-h-[400px] flex items-center">
                    <!-- Background Graphic -->
                    <div class="absolute inset-0 opacity-30">
                        <div class="absolute bottom-0 left-0 right-0 h-64 bg-gradient-to-t from-blue-900/50 to-transparent"></div>
                         <!-- Abstract globe/mesh placeholder -->
                        <svg class="absolute bottom-0 w-full h-full text-blue-900/20" viewBox="0 0 100 100" preserveAspectRatio="none">
                            <path d="M0 100 Q 50 50 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                            <path d="M0 100 Q 50 40 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                            <path d="M0 100 Q 50 30 100 100" fill="none" stroke="currentColor" stroke-width="0.5" />
                        </svg>
                    </div>

                    <div class="relative z-10 p-16 w-full grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                        <div>
                            <h2 class="text-3xl font-light mb-6">
                                AIUC-1 is the world's first<br>standard for AI agents
                            </h2>
                            <p class="text-sm text-gray-400 mb-8 max-w-md">
                                AIUC-1 covers data & privacy, security, safety, reliability, accountability and societal risks.
                            </p>
                            <button class="bg-white text-black px-6 py-2 text-xs font-medium rounded-sm hover:bg-gray-200 transition-colors">
                                Explore AIUC-1
                            </button>
                        </div>
                        <div class="flex justify-end">
                            <div class="w-48 h-64 bg-gradient-to-br from-gray-200 to-gray-400 rounded-lg p-1 shadow-2xl rotate-3 transform hover:rotate-0 transition-transform duration-500">
                                <div class="w-full h-full bg-white/10 backdrop-blur-md border border-white/20 rounded flex flex-col items-center justify-between p-4">
                                    <div class="w-12 h-12 rounded-full border-2 border-white/30 flex items-center justify-center">
                                        <div class="w-8 h-8 rounded-full bg-white/20"></div>
                                    </div>
                                    <div class="text-center">
                                        <div class="text-[10px] uppercase tracking-widest text-white/70 mb-1">Standard</div>
                                        <div class="text-xl font-bold text-white tracking-tighter">AIUC-1</div>
                                        <div class="text-[8px] uppercase tracking-wider text-white/50 mt-1">Certification</div>
                                    </div>
                                    <div class="w-full h-8 bg-white/10 rounded-sm"></div>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- Testimonials -->
                <section>
                    <div class="flex justify-between items-baseline mb-16 border-b border-gray-100 pb-4">
                        <h2 class="text-3xl font-light text-gray-900">
                            Embrace AI with confidence
                        </h2>
                        <span class="text-[10px] text-gray-400 uppercase tracking-wider">Testimonials</span>
                    </div>

                    <div class="relative">
                        <div class="flex gap-8 overflow-hidden">
                            <div class="w-full md:w-[800px] shrink-0 bg-gray-50 flex">
                                <div class="w-1/3 shrink-0">
                                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?q=80&w=400&auto=format&fit=crop" alt="Phil Venables" class="w-full h-full object-cover grayscale" />
                                </div>
                                <div class="w-2/3 p-12 flex flex-col justify-center">
                                    <blockquote class="text-xl font-light leading-relaxed mb-8">
                                        "We need a SOC 2 for AI agents - a familiar, actionable standard for security and trust."
                                    </blockquote>
                                    <div class="flex items-center gap-2">
                                        <div class="w-4 h-4 bg-yellow-400 rounded-full"></div> <!-- Placeholder for Google Cloud logo -->
                                        <span class="text-xs font-semibold text-gray-500">Google Cloud</span>
                                    </div>
                                    <div class="mt-2">
                                        <div class="font-medium">Phil Venables</div>
                                        <div class="text-xs text-gray-500">Former CISO</div>
                                    </div>
                                </div>
                            </div>
                            <!-- Next slide preview -->
                            <div class="w-1/3 shrink-0 opacity-50">
                                <img src="https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?q=80&w=400&auto=format&fit=crop" alt="Next testimonial" class="w-full h-full object-cover grayscale" />
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
            AIUC
        </div>

        <div class="max-w-[1600px] mx-auto px-6 relative z-10">
            <div class="flex flex-col md:flex-row justify-between items-end md:items-center mb-24">
                <div class="text-lg font-light">Move with confidence</div>
                <div class="text-lg font-light underline decoration-1 underline-offset-4">AIUC.COM</div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-12 gap-8 items-end">
                <div class="md:col-span-6">
                    <!-- Logo -->
                    <div class="flex items-center gap-4 mb-4">
                        <div class="w-8 h-8 rounded-full border border-black flex items-center justify-center">
                            <div class="w-1 h-1 bg-black rounded-full"></div>
                        </div>
                        <div class="text-sm font-medium leading-tight">
                            Artificial Intelligence<br>Underwriting Company
                        </div>
                    </div>
                </div>
                
                <div class="md:col-span-6 flex flex-col md:flex-row justify-between items-end md:items-end gap-8">
                    <div class="text-[10px] text-gray-400">
                        © 2025 AIUC
                    </div>
                    
                    <div class="flex gap-8 text-[10px] font-medium uppercase tracking-wide">
                        <div class="flex flex-col gap-2">
                            <a href="#">Team</a>
                            <a href="#">Research</a>
                            <a href="#">Contact</a>
                        </div>
                        <div class="flex flex-col gap-2">
                            <a href="#">Terms</a>
                            <a href="#">Privacy Policy</a>
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

