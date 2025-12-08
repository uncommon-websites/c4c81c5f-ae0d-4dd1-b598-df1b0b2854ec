<script>
    import Navbar from '$lib/components/Navbar.svelte';
    import Footer from '$lib/components/Footer.svelte';
    import FeatureRow from '$lib/components/FeatureRow.svelte';
</script>

<div class="bg-[var(--color-canopy-dark)] min-h-screen flex flex-col">
    <Navbar />

    <main class="flex-grow">
        <!-- Hero Section -->
        <section class="relative pt-32 pb-20 overflow-hidden">
            <div class="container mx-auto px-6 relative z-10">
                <div class="max-w-4xl mx-auto text-center">
                    <!-- Search/Notification Pill -->
                    <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm border border-white/10 rounded-full px-4 py-1.5 mb-8">
                        <span class="w-2 h-2 rounded-full bg-[var(--color-canopy-lime)]"></span>
                        <span class="text-white text-sm font-medium">Canopy 2.0</span>
                        <span class="text-gray-400 text-sm">is here</span>
                        <svg class="w-4 h-4 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg>
                    </div>

                    <h1 class="text-5xl md:text-7xl font-bold text-white tracking-tight mb-6 text-balance">
                        Build better B2B lending products.
                    </h1>
                    
                    <p class="text-lg md:text-xl text-gray-400 mb-10 max-w-2xl mx-auto leading-relaxed text-balance">
                        The most flexible loan management system for commercial lenders. Get everything you need to operate & scale secured lending, installment, and hybrid products. Your secret weapon for everything post-origination.
                    </p>
                    
                    <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                        <button class="bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2">
                            Get started
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14M12 5l7 7-7 7"/>
                            </svg>
                        </button>
                        <button class="bg-transparent border border-white/20 hover:bg-white/10 text-white px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2">
                            Explore Canopy 2.0
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14M12 5l7 7-7 7"/>
                            </svg>
                        </button>
                    </div>
                </div>
            </div>

            <!-- Hero Images/Cards -->
            <div class="mt-20 relative">
                <div class="flex justify-center gap-6 overflow-hidden px-6">
                    <!-- Card 1 -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 transform -rotate-2 mt-8">
                        <div class="bg-white p-4">
                            <div class="flex items-center justify-between mb-4">
                                <div class="h-2 w-20 bg-gray-200 rounded"></div>
                                <div class="h-8 w-24 bg-[var(--color-canopy-lime)]/20 rounded text-[var(--color-canopy-lime)] text-xs flex items-center justify-center font-bold">$1,544.45</div>
                            </div>
                            <div class="space-y-3">
                                <div class="h-24 bg-gray-100 rounded-lg w-full"></div>
                                <div class="h-4 w-full bg-gray-50 rounded"></div>
                                <div class="h-4 w-2/3 bg-gray-50 rounded"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Card 2 (Center) -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 z-10">
                        <div class="bg-white h-full flex flex-col">
                            <div class="bg-[var(--color-canopy-lime)] p-6">
                                <div class="flex justify-between items-center">
                                    <div class="h-6 w-24 bg-black/10 rounded"></div>
                                    <div class="h-8 w-8 bg-black/10 rounded-full"></div>
                                </div>
                            </div>
                            <div class="p-6 flex-grow">
                                <div class="flex gap-4 mb-6">
                                    <div class="w-1/3 space-y-2">
                                        <div class="h-2 w-full bg-gray-100 rounded"></div>
                                        <div class="h-2 w-2/3 bg-gray-100 rounded"></div>
                                    </div>
                                    <div class="w-2/3 space-y-2">
                                        <div class="h-8 w-full bg-gray-50 rounded border border-gray-100"></div>
                                        <div class="h-2 w-full bg-gray-100 rounded mt-2"></div>
                                        <div class="h-2 w-full bg-gray-100 rounded"></div>
                                        <div class="h-2 w-full bg-gray-100 rounded"></div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Card 3 -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 transform rotate-2 mt-8">
                        <div class="bg-white p-4">
                            <div class="flex items-center justify-between mb-4">
                                <div class="h-2 w-20 bg-gray-200 rounded"></div>
                                <div class="h-8 w-24 bg-[var(--color-canopy-lime)]/20 rounded text-[var(--color-canopy-lime)] text-xs flex items-center justify-center font-bold">$1,544.45</div>
                            </div>
                            <div class="space-y-3">
                                <div class="h-24 bg-gray-100 rounded-lg w-full"></div>
                                <div class="h-4 w-full bg-gray-50 rounded"></div>
                                <div class="h-4 w-2/3 bg-gray-50 rounded"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Logos Section -->
        <section class="py-12 border-y border-white/5 bg-black/20">
            <div class="container mx-auto px-6">
                <div class="flex flex-wrap justify-center items-center gap-12 md:gap-20 opacity-50 grayscale">
                    <!-- Novo -->
                    <svg class="h-6 md:h-8 w-auto text-white" viewBox="0 0 100 30" fill="currentColor">
                        <path d="M10,5 L15,5 L15,25 L10,25 L10,5 Z M25,5 L40,5 L40,10 L30,10 L30,20 L40,20 L40,25 L25,25 L25,5 Z M50,5 L55,5 L60,25 L55,25 L52.5,15 L50,25 L45,25 L50,5 Z M70,5 L85,5 L85,25 L70,25 L70,20 L80,20 L80,10 L70,10 L70,5 Z" />
                    </svg>
                    <!-- Mercury -->
                    <svg class="h-6 md:h-8 w-auto text-white" viewBox="0 0 100 30" fill="currentColor">
                         <circle cx="15" cy="15" r="10" />
                         <rect x="35" y="5" width="50" height="20" />
                    </svg>
                    <!-- Bluevine -->
                    <svg class="h-6 md:h-8 w-auto text-white" viewBox="0 0 100 30" fill="currentColor">
                        <rect x="10" y="10" width="20" height="10" />
                        <rect x="40" y="5" width="50" height="20" />
                    </svg>
                    <!-- Flexport -->
                    <svg class="h-6 md:h-8 w-auto text-white" viewBox="0 0 100 30" fill="currentColor">
                        <path d="M10,5 L30,5 L30,10 L15,10 L15,12.5 L25,12.5 L25,17.5 L15,17.5 L15,25 L10,25 L10,5 Z" />
                         <rect x="40" y="5" width="50" height="20" />
                    </svg>
                    <!-- Prime -->
                    <svg class="h-6 md:h-8 w-auto text-white" viewBox="0 0 100 30" fill="currentColor">
                        <rect x="10" y="5" width="80" height="20" />
                    </svg>
                </div>
            </div>
        </section>

        <!-- Canopy Core Section -->
        <section class="py-32 relative overflow-hidden">
            <div class="container mx-auto px-6 relative z-10">
                <div class="text-center mb-24">
                    <h2 class="text-[var(--color-canopy-lime)] font-mono text-xs tracking-[0.2em] uppercase mb-6">Canopy Core</h2>
                    <h3 class="text-4xl md:text-6xl font-bold text-white mb-2 tracking-tight">A loan management system.</h3>
                    <h3 class="text-4xl md:text-6xl font-bold text-gray-600 tracking-tight">And so much more.</h3>
                </div>

                <div class="grid md:grid-cols-2 gap-16 items-center max-w-6xl mx-auto">
                    <!-- Purple Card -->
                    <div class="bg-gradient-to-br from-[#7C3AED] to-[#4C1D95] rounded-3xl p-12 aspect-[4/3] relative overflow-hidden flex items-center justify-center shadow-2xl">
                        <!-- Abstract UI Elements -->
                        <div class="relative z-10 w-full max-w-[320px]">
                            <!-- Credit Card -->
                            <div class="bg-white/10 backdrop-blur-xl border border-white/20 rounded-2xl p-6 mb-8 shadow-xl relative overflow-hidden group hover:scale-105 transition-transform duration-500">
                                <div class="absolute top-0 right-0 p-6 opacity-50">
                                    <svg class="w-12 h-8 text-white" viewBox="0 0 48 32" fill="currentColor">
                                        <path d="M32 0H16C7.163 0 0 7.163 0 16s7.163 16 16 16h16c8.837 0 16-7.163 16-16S40.837 0 32 0z" fill-opacity="0.5"/>
                                        <circle cx="16" cy="16" r="16" fill-opacity="0.5"/>
                                    </svg>
                                </div>
                                <div class="w-12 h-8 bg-[#D4AF37] rounded-md mb-8 relative z-10"></div>
                                <div class="space-y-1 relative z-10">
                                    <div class="text-white/60 text-[10px] uppercase tracking-wider font-medium">Card Holder</div>
                                    <div class="text-white font-mono text-lg tracking-widest">ARLENE MCCOY</div>
                                </div>
                                <div class="absolute bottom-6 right-6 text-white font-bold italic text-2xl">VISA</div>
                            </div>
                            
                            <!-- Floating Pills -->
                            <div class="relative">
                                <div class="absolute -left-4 top-0 bg-white text-black px-5 py-2.5 rounded-full text-sm font-semibold shadow-lg flex items-center gap-2 transform -rotate-2">
                                    <div class="w-5 h-5 rounded-full bg-blue-100 flex items-center justify-center text-blue-600">
                                        <svg class="w-3 h-3" fill="currentColor" viewBox="0 0 20 20"><path d="M4 4a2 2 0 012-2h4.586A2 2 0 0112 2.586L15.414 6A2 2 0 0116 7.414V16a2 2 0 01-2 2H6a2 2 0 01-2-2V4z"/></svg>
                                    </div>
                                    Installment loans
                                </div>
                                <div class="absolute -right-4 top-12 bg-white/10 backdrop-blur-md text-white px-5 py-2.5 rounded-full text-sm font-semibold border border-white/20 flex items-center gap-2 transform rotate-2">
                                    <div class="w-5 h-5 rounded-full bg-purple-500/30 flex items-center justify-center text-purple-200">
                                        <svg class="w-3 h-3" fill="currentColor" viewBox="0 0 20 20"><path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3zM6 8a2 2 0 11-4 0 2 2 0 014 0zM16 18v-3a5.972 5.972 0 00-.75-2.906A3.005 3.005 0 0119 15v3h-3zM4.75 12.094A5.973 5.973 0 004 15v3H1v-3a3 3 0 013.75-2.906z"/></svg>
                                    </div>
                                    Working capital
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Text Content -->
                    <div class="space-y-8">
                        <h3 class="text-4xl md:text-5xl font-bold text-white tracking-tight">Scale with flexibility.</h3>
                        <p class="text-gray-400 text-lg leading-relaxed max-w-lg">
                            Things change. Markets and borrower needs evolve. Canopy provides modern lending built to adapt and grow with you and your customers.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- White Section -->
        <div class="bg-[#F9FAFB] text-black rounded-t-[4rem] relative z-20 mt-[-2rem] pt-32 pb-32">
            <div class="container mx-auto px-6">
                <!-- Header -->
                <div class="max-w-4xl mb-24">
                    <div class="flex items-center gap-4 mb-6">
                        <div class="h-px w-12 bg-gray-300"></div>
                        <span class="text-gray-500 font-mono text-xs tracking-[0.2em] uppercase">CanopyOS</span>
                    </div>
                    <h2 class="text-4xl md:text-6xl font-bold text-gray-900 mb-2 tracking-tight">One home for operating and scaling lending products.</h2>
                    <h2 class="text-4xl md:text-6xl font-bold text-gray-400 tracking-tight mb-8">However complex.</h2>
                    
                    <a href="#" class="inline-flex items-center gap-2 text-sm font-semibold border-b border-black pb-0.5 hover:text-gray-600 transition-colors">
                        Explore our platform
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </a>
                </div>

                <!-- Features Grid -->
                <div class="flex flex-col lg:flex-row gap-12">
                    <!-- Sidebar Navigation (Sticky) -->
                    <div class="hidden lg:block w-64 flex-shrink-0">
                        <div class="sticky top-32 space-y-4">
                            <div class="flex items-center gap-2 text-sm font-semibold text-black border-l-2 border-black pl-4 py-1">
                                <span class="w-1.5 h-1.5 rounded-full bg-[var(--color-canopy-lime)]"></span>
                                Collateral Management
                            </div>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Canopy Connect</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">DataDirect</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">LoanLab</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Preview</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">SafeGuard</a>
                        </div>
                    </div>

                    <!-- Feature Cards -->
                    <div class="flex-grow space-y-8">
                        <FeatureRow 
                            title="Collateral Management" 
                            description="Unify your loan tape with collateral. Canopy is the only LMS that seamlessly integrates loan tapes with collateral, streamlining secured lending processes."
                            icon="lock"
                            image="collateral"
                        />
                         <FeatureRow 
                            title="Canopy Connect" 
                            description="Drop manual work. Canopy Connect lets you design custom workflows that automate loan tasks, so you can spend your time on other things."
                            icon="connect"
                            image="connect"
                        />
                         <FeatureRow 
                            title="DataDirect" 
                            description="Present the insights that matter. Generate ready-made reports that steer your upsell or cross-sell strategy. DataDirect makes your loan account insights count."
                            icon="data"
                            image="data"
                        />
                         <FeatureRow 
                            title="LoanLab" 
                            description="Innovate, simulate, operate. Simulate the entire lifecycle of a loan, test different policies and actions, and observe the effects over time (and in real time)."
                            icon="lab"
                            image="lab"
                        />
                         <FeatureRow 
                            title="Preview" 
                            description="Get ahead of borrowing decisions. Preview an account before committing major changes to production, creating more transparency and better decision-making."
                            icon="preview"
                            image="preview"
                        />
                         <FeatureRow 
                            title="SafeGuard" 
                            description="Get accurate calculations. Align all calculations with the business lending scenarios and edge cases that matter via always-on SafeGuard tests."
                            icon="guard"
                            image="guard"
                        />
                    </div>
                </div>

                <!-- Embed Section -->
                <div class="mt-32 text-center max-w-4xl mx-auto mb-24">
                    <div class="w-24 h-24 mx-auto bg-gradient-to-br from-blue-100 to-purple-100 rounded-full flex items-center justify-center mb-8 relative">
                        <div class="absolute inset-0 bg-white/50 blur-xl rounded-full"></div>
                        <svg class="w-10 h-10 text-blue-600 relative z-10" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.384-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z"></path></svg>
                    </div>
                    <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8 leading-tight">
                        Embed modern lending and credit products — whether you're a fintech, digital bank, or vertical SaaS company.
                    </h2>
                    <button class="bg-white border border-gray-200 hover:border-gray-400 text-black px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2 mx-auto">
                        Explore use cases
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </button>
                </div>

                <!-- Trusted By Section -->
                <div class="mb-32">
                    <p class="text-xl text-gray-500 mb-12">Trusted by modern lending teams. Learn more from our customers.</p>
                    
                    <div class="grid md:grid-cols-3 gap-6">
                        <!-- Flexport Card (Large) -->
                        <div class="md:col-span-2 bg-[#0A0A0A] rounded-3xl p-10 relative overflow-hidden group min-h-[400px] flex flex-col justify-end">
                            <div class="absolute inset-0 bg-gradient-to-t from-black via-black/50 to-transparent"></div>
                            
                            <div class="relative z-10">
                                <div class="flex items-center gap-4 mb-6">
                                    <div class="text-white font-bold text-2xl tracking-tight">flexport.</div>
                                    <div class="w-8 h-8 rounded-full bg-[var(--color-canopy-lime)] flex items-center justify-center text-black font-bold">+</div>
                                    <div class="flex items-center gap-2 text-white font-semibold text-xl tracking-tight">
                                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path d="M12 2L2 7L12 12L22 7L12 2Z" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                                            <path d="M2 17L12 22L22 17" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                                            <path d="M2 12L12 17L22 12" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                                        </svg>
                                        Canopy
                                    </div>
                                </div>
                                <h3 class="text-3xl font-bold text-white mb-4 max-w-md">
                                    <span class="text-[#F5A623]">flexport.</span><br>
                                    How Flexport leveraged Canopy to scale its lending program
                                </h3>
                                <div class="w-10 h-10 rounded-full bg-white/10 backdrop-blur-md border border-white/20 flex items-center justify-center text-white group-hover:bg-white group-hover:text-black transition-colors">
                                    <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
                                </div>
                            </div>
                        </div>

                        <!-- Smaller Cards -->
                        <div class="space-y-6">
                            <!-- Card 2 -->
                            <div class="bg-[#0A0A0A] rounded-3xl p-8 relative overflow-hidden group h-[240px] flex flex-col justify-end">
                                <div class="absolute inset-0 bg-gradient-to-br from-blue-900/40 to-black"></div>
                                <div class="relative z-10 flex justify-between items-end">
                                    <div class="w-12 h-12 rounded-full bg-yellow-400/20 blur-xl absolute -left-2 -bottom-2"></div>
                                    <div class="w-10 h-10 rounded-full bg-white/10 backdrop-blur-md border border-white/20 flex items-center justify-center text-white group-hover:bg-white group-hover:text-black transition-colors ml-auto">
                                        <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
                                    </div>
                                </div>
                            </div>
                            <!-- Card 3 -->
                            <div class="bg-[#0A0A0A] rounded-3xl p-8 relative overflow-hidden group h-[240px] flex flex-col justify-end">
                                <div class="absolute inset-0 bg-gradient-to-br from-green-900/40 to-black"></div>
                                <div class="relative z-10 flex justify-between items-end">
                                    <div class="w-12 h-12 rounded-full bg-green-400/20 blur-xl absolute -left-2 -bottom-2"></div>
                                    <div class="w-10 h-10 rounded-full bg-white/10 backdrop-blur-md border border-white/20 flex items-center justify-center text-white group-hover:bg-white group-hover:text-black transition-colors ml-auto">
                                        <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Banner -->
                <div class="bg-[#0A0A0A] rounded-3xl p-12 md:p-20 relative overflow-hidden mb-32 text-center">
                    <div class="absolute inset-0 bg-[url('/grid-pattern.svg')] opacity-10"></div>
                    <div class="absolute left-0 top-0 w-64 h-64 bg-yellow-500/10 blur-[100px] rounded-full"></div>
                    <div class="absolute right-0 bottom-0 w-64 h-64 bg-blue-500/10 blur-[100px] rounded-full"></div>
                    
                    <div class="relative z-10 max-w-3xl mx-auto">
                        <h2 class="text-4xl md:text-6xl font-bold text-white mb-6 tracking-tight">
                            Create flexible lending products. <span class="text-[var(--color-canopy-lime)]">With less work.</span>
                        </h2>
                        <p class="text-gray-400 mb-10">
                            Purpose built for developers, our modern, low-code API lets you launch fast and scale with ease.
                        </p>
                        <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-md border border-white/10 rounded-full px-4 py-2 text-white text-sm hover:bg-white/20 transition-colors cursor-pointer">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
                            Canopy Docs
                            <kbd class="bg-black/30 px-1.5 py-0.5 rounded text-xs text-gray-400 font-mono">K</kbd>
                        </div>
                    </div>
                </div>

                <!-- Integrations -->
                <div class="text-center mb-32">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
                        Card issuers. Payments processors.<br>
                        Credit reporting. <span class="text-gray-400">Whoever you're<br>partnered with, Canopy connects.</span>
                    </h2>
                    <button class="bg-gray-100 hover:bg-gray-200 text-black px-6 py-2 rounded-full text-sm font-medium transition-colors flex items-center gap-2 mx-auto mb-16 mt-8">
                        Explore all integrations
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </button>

                    <div class="grid grid-cols-2 md:grid-cols-4 gap-px bg-gray-200 border border-gray-200 rounded-2xl overflow-hidden">
                        {#each ['checkout.com', 'dwolla', 'modern treasury', 'stripe', 'galileo', 'intercom', 'square', 'tableau'] as logo}
                        <div class="bg-[#F9FAFB] p-12 flex items-center justify-center grayscale opacity-60 hover:grayscale-0 hover:opacity-100 transition-all duration-300">
                            <span class="font-bold text-xl uppercase tracking-wider">{logo}</span>
                        </div>
                        {/each}
                    </div>
                </div>

                <!-- Blog Section -->
                <div class="mb-12">
                    <h2 class="text-4xl font-bold text-gray-900 mb-12">Learn more about next-gen lending.</h2>
                    <div class="grid md:grid-cols-2 gap-8">
                        <!-- Post 1 -->
                        <div class="group cursor-pointer">
                            <div class="bg-gradient-to-br from-gray-200 to-gray-300 rounded-3xl aspect-[16/9] mb-6 relative overflow-hidden">
                                <div class="absolute inset-0 flex items-center justify-center">
                                    <div class="grid grid-cols-6 gap-4 opacity-50">
                                        {#each Array(24) as _}
                                            <svg class="w-6 h-6 text-blue-600 transform -rotate-45" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 10l7-7m0 0l7 7m-7-7v18"></path></svg>
                                        {/each}
                                    </div>
                                </div>
                            </div>
                            <div class="text-xs font-bold text-gray-500 uppercase tracking-wider mb-2">Industry Insights</div>
                            <h3 class="text-2xl font-bold text-gray-900 group-hover:text-blue-600 transition-colors">Middle-market lending is a windfall for non-bank lenders</h3>
                        </div>
                        <!-- Post 2 -->
                        <div class="group cursor-pointer">
                            <div class="bg-gray-100 rounded-3xl aspect-[16/9] mb-6 relative overflow-hidden flex items-center justify-center">
                                <div class="flex gap-4">
                                    <div class="w-16 h-16 rounded-full bg-green-400 blur-xl opacity-80"></div>
                                    <div class="w-20 h-20 rounded-full bg-blue-400 blur-xl opacity-80"></div>
                                    <div class="w-12 h-12 rounded-full bg-purple-400 blur-xl opacity-80"></div>
                                </div>
                            </div>
                            <div class="text-xs font-bold text-gray-500 uppercase tracking-wider mb-2">Industry Insights</div>
                            <h3 class="text-2xl font-bold text-gray-900 group-hover:text-blue-600 transition-colors">The loan lifecycle: From origination to payoff</h3>
                        </div>
                    </div>
                </div>


    </main>

    <Footer />
</div>

