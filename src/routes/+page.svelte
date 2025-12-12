<script>
    import Navbar from '$lib/components/Navbar.svelte';
    import Footer from '$lib/components/Footer.svelte';
    import FeatureRow from '$lib/components/FeatureRow.svelte';
</script>

<div class="bg-[var(--color-primary-dark)] min-h-screen flex flex-col">
    <Navbar />

    <main class="flex-grow">
        <!-- Hero Section -->
        <section class="relative pt-32 pb-20 overflow-hidden">
            <div class="container mx-auto px-6 relative z-10">
                <div class="max-w-4xl mx-auto text-center">
                    <!-- Search/Notification Pill -->
                    <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm border border-white/10 rounded-full px-4 py-1.5 mb-8">
                        <span class="w-2 h-2 rounded-full bg-[var(--color-primary-500)]"></span>
                        <span class="text-white text-sm font-medium">Built for Canada</span>
                        <span class="text-gray-400 text-sm">Trusted by dealers</span>
                        <svg class="w-4 h-4 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg>
                    </div>

                    <h1 class="text-5xl md:text-7xl font-bold text-white tracking-tight mb-6 text-balance">
                        Modern lending tools for dealers and lenders.
                    </h1>
                    
                    <p class="text-lg md:text-xl text-gray-400 mb-10 max-w-2xl mx-auto leading-relaxed text-balance">
                        Streamline credit applications, connect with multiple lenders, and close deals faster. The complete platform for automotive and mortgage finance managers across Canada.
                    </p>
                    
                    <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                        <button class="bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2">
                            Get started
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14M12 5l7 7-7 7"/>
                            </svg>
                        </button>
                        <button class="bg-transparent border border-white/20 hover:bg-white/10 text-white px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2">
                            Watch demo
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
                                <div class="text-xs font-semibold text-gray-500">Credit Application</div>
                                <div class="h-8 w-24 bg-[var(--color-primary-500)]/20 rounded text-[var(--color-primary-600)] text-xs flex items-center justify-center font-bold">Approved</div>
                            </div>
                            <div class="space-y-3">
                                <div class="h-24 bg-gray-100 rounded-lg w-full flex items-center justify-center">
                                    <div class="text-center">
                                        <div class="text-2xl font-bold text-gray-800">$45,000</div>
                                        <div class="text-xs text-gray-500">Loan Amount</div>
                                    </div>
                                </div>
                                <div class="h-4 w-full bg-gray-50 rounded"></div>
                                <div class="h-4 w-2/3 bg-gray-50 rounded"></div>
                            </div>
                        </div>
                    </div>

                    <!-- Card 2 (Center) -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 z-10">
                        <div class="bg-white h-full flex flex-col">
                            <div class="bg-[var(--color-primary-500)] p-6">
                                <div class="flex justify-between items-center">
                                    <div class="text-black font-bold">Deal Summary</div>
                                    <div class="h-8 w-8 bg-black/10 rounded-full"></div>
                                </div>
                            </div>
                            <div class="p-6 flex-grow">
                                <div class="space-y-4">
                                    <div class="flex justify-between">
                                        <span class="text-sm text-gray-500">Vehicle Price</span>
                                        <span class="text-sm font-semibold">$42,500</span>
                                    </div>
                                    <div class="flex justify-between">
                                        <span class="text-sm text-gray-500">Down Payment</span>
                                        <span class="text-sm font-semibold">$8,500</span>
                                    </div>
                                    <div class="flex justify-between">
                                        <span class="text-sm text-gray-500">Term</span>
                                        <span class="text-sm font-semibold">60 months</span>
                                    </div>
                                    <div class="h-px bg-gray-200"></div>
                                    <div class="flex justify-between">
                                        <span class="text-sm font-bold">Monthly Payment</span>
                                        <span class="text-lg font-bold text-[var(--color-primary-600)]">$645</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Card 3 -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 transform rotate-2 mt-8">
                        <div class="bg-white p-4">
                            <div class="flex items-center justify-between mb-4">
                                <div class="text-xs font-semibold text-gray-500">Lender Response</div>
                                <div class="h-8 w-24 bg-green-100 rounded text-green-700 text-xs flex items-center justify-center font-bold">3.9% APR</div>
                            </div>
                            <div class="space-y-3">
                                <div class="h-24 bg-gray-100 rounded-lg w-full flex items-center justify-center">
                                    <div class="text-center">
                                        <div class="text-xs text-gray-500 mb-1">Response Time</div>
                                        <div class="text-2xl font-bold text-gray-800">2 min</div>
                                    </div>
                                </div>
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
                <p class="text-center text-gray-500 text-sm mb-8">Trusted by leading Canadian dealerships and lenders</p>
                <div class="flex flex-wrap justify-center items-center gap-12 md:gap-20 opacity-50 grayscale">
                    <!-- Placeholder Logos -->
                    <div class="h-8 w-32 bg-white/20 rounded"></div>
                    <div class="h-8 w-28 bg-white/20 rounded"></div>
                    <div class="h-8 w-36 bg-white/20 rounded"></div>
                    <div class="h-8 w-32 bg-white/20 rounded"></div>
                    <div class="h-8 w-28 bg-white/20 rounded"></div>
                </div>
            </div>
        </section>

        <!-- CreditApp Core Section -->
        <section class="py-32 relative overflow-hidden">
            <div class="container mx-auto px-6 relative z-10">
                <div class="text-center mb-24">
                    <h2 class="text-[var(--color-primary-500)] font-mono text-xs tracking-[0.2em] uppercase mb-6">CreditApp Platform</h2>
                    <h3 class="text-4xl md:text-6xl font-bold text-white mb-2 tracking-tight">Credit applications made simple.</h3>
                    <h3 class="text-4xl md:text-6xl font-bold text-gray-600 tracking-tight">Approvals made faster.</h3>
                </div>

                <div class="grid md:grid-cols-2 gap-16 items-center max-w-6xl mx-auto">
                    <!-- Teal Card -->
                    <div class="bg-gradient-to-br from-[#0D9488] to-[#115E59] rounded-3xl p-12 aspect-[4/3] relative overflow-hidden flex items-center justify-center shadow-2xl">
                        <!-- Abstract UI Elements -->
                        <div class="relative z-10 w-full max-w-[320px]">
                            <!-- Application Card -->
                            <div class="bg-white/10 backdrop-blur-xl border border-white/20 rounded-2xl p-6 mb-8 shadow-xl relative overflow-hidden group hover:scale-105 transition-transform duration-500">
                                <div class="space-y-4 relative z-10">
                                    <div class="flex justify-between items-center">
                                        <div class="text-white/60 text-xs uppercase tracking-wider font-medium">Application Status</div>
                                        <div class="bg-green-400 text-green-900 px-3 py-1 rounded-full text-xs font-bold">Approved</div>
                                    </div>
                                    <div class="text-white font-bold text-3xl">$45,000</div>
                                    <div class="h-px bg-white/20"></div>
                                    <div class="grid grid-cols-2 gap-4">
                                        <div>
                                            <div class="text-white/60 text-[10px] uppercase">Term</div>
                                            <div class="text-white font-semibold">60 months</div>
                                        </div>
                                        <div>
                                            <div class="text-white/60 text-[10px] uppercase">Rate</div>
                                            <div class="text-white font-semibold">3.9%</div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <!-- Floating Pills -->
                            <div class="relative">
                                <div class="absolute -left-4 top-0 bg-white text-black px-5 py-2.5 rounded-full text-sm font-semibold shadow-lg flex items-center gap-2 transform -rotate-2">
                                    <div class="w-5 h-5 rounded-full bg-blue-100 flex items-center justify-center text-blue-600">
                                        <svg class="w-3 h-3" fill="currentColor" viewBox="0 0 20 20"><path d="M9 2a1 1 0 000 2h2a1 1 0 100-2H9z M4 5a2 2 0 012-2 3 3 0 003 3h2a3 3 0 003-3 2 2 0 012 2v11a2 2 0 01-2 2H6a2 2 0 01-2-2V5z"/></svg>
                                    </div>
                                    Auto loans
                                </div>
                                <div class="absolute -right-4 top-12 bg-white/10 backdrop-blur-md text-white px-5 py-2.5 rounded-full text-sm font-semibold border border-white/20 flex items-center gap-2 transform rotate-2">
                                    <div class="w-5 h-5 rounded-full bg-teal-500/30 flex items-center justify-center text-teal-200">
                                        <svg class="w-3 h-3" fill="currentColor" viewBox="0 0 20 20"><path d="M10.707 2.293a1 1 0 00-1.414 0l-7 7a1 1 0 001.414 1.414L4 10.414V17a1 1 0 001 1h2a1 1 0 001-1v-2a1 1 0 011-1h2a1 1 0 011 1v2a1 1 0 001 1h2a1 1 0 001-1v-6.586l.293.293a1 1 0 001.414-1.414l-7-7z"/></svg>
                                    </div>
                                    Mortgages
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Text Content -->
                    <div class="space-y-8">
                        <h3 class="text-4xl md:text-5xl font-bold text-white tracking-tight">Close deals faster with confidence.</h3>
                        <p class="text-gray-400 text-lg leading-relaxed max-w-lg">
                            Connect to multiple lenders instantly, get real-time credit decisions, and provide your customers with the best financing options. Built specifically for Canadian dealers and finance managers.
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
                        <span class="text-gray-500 font-mono text-xs tracking-[0.2em] uppercase">Platform Features</span>
                    </div>
                    <h2 class="text-4xl md:text-6xl font-bold text-gray-900 mb-2 tracking-tight">Everything you need to streamline credit applications.</h2>
                    <h2 class="text-4xl md:text-6xl font-bold text-gray-400 tracking-tight mb-8">All in one place.</h2>
                    
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
                                <span class="w-1.5 h-1.5 rounded-full bg-[var(--color-primary-500)]"></span>
                                Credit Applications
                            </div>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Lender Network</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Deal Structuring</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Document Manager</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Compliance</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Analytics</a>
                        </div>
                    </div>

                    <!-- Feature Cards -->
                    <div class="flex-grow space-y-8">
                        <FeatureRow 
                            title="Credit Applications" 
                            description="Submit once, reach multiple lenders. Our streamlined application process connects you with our entire lender network instantly, saving time and increasing approval rates."
                            icon="lock"
                            image="collateral"
                        />
                         <FeatureRow 
                            title="Lender Network" 
                            description="Access Canada's best rates. Connect with major banks, credit unions, and alternative lenders all in one platform. Get competitive offers in real-time."
                            icon="connect"
                            image="connect"
                        />
                         <FeatureRow 
                            title="Deal Structuring" 
                            description="Build the perfect deal. Compare multiple financing scenarios side-by-side, adjust terms on the fly, and present customers with options that work for their budget."
                            icon="data"
                            image="data"
                        />
                         <FeatureRow 
                            title="Document Manager" 
                            description="Go paperless, stay organized. Upload, store, and share all required documents securely. E-signature integration makes closing deals faster than ever."
                            icon="lab"
                            image="lab"
                        />
                         <FeatureRow 
                            title="Compliance" 
                            description="Stay compliant automatically. Built-in checks ensure every application meets Canadian lending regulations. Audit trails and reporting keep you protected."
                            icon="preview"
                            image="preview"
                        />
                         <FeatureRow 
                            title="Analytics" 
                            description="Make data-driven decisions. Track approval rates, average deal size, lender performance, and more. Insights that help you optimize your finance department."
                            icon="guard"
                            image="guard"
                        />
                    </div>
                </div>

                <!-- Integration Section -->
                <div class="mt-32 text-center max-w-4xl mx-auto mb-24">
                    <div class="w-24 h-24 mx-auto bg-gradient-to-br from-teal-100 to-cyan-100 rounded-full flex items-center justify-center mb-8 relative">
                        <div class="absolute inset-0 bg-white/50 blur-xl rounded-full"></div>
                        <svg class="w-10 h-10 text-teal-600 relative z-10" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                    </div>
                    <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8 leading-tight">
                        Seamlessly integrate with your existing dealership management system.
                    </h2>
                    <button class="bg-white border border-gray-200 hover:border-gray-400 text-black px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2 mx-auto">
                        View integrations
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </button>
                </div>

                <!-- Trusted By Section -->
                <div class="mb-32">
                    <p class="text-xl text-gray-500 mb-12">Trusted by Canadian dealers. See how they're closing more deals.</p>
                    
                    <div class="grid md:grid-cols-3 gap-6">
                        <!-- Featured Dealer Card (Large) -->
                        <div class="md:col-span-2 bg-[#0A0A0A] rounded-3xl p-10 relative overflow-hidden group min-h-[400px] flex flex-col justify-end">
                            <div class="absolute inset-0 bg-gradient-to-t from-black via-black/50 to-transparent"></div>
                            
                            <div class="relative z-10">
                                <div class="flex items-center gap-4 mb-6">
                                    <div class="text-white font-bold text-2xl tracking-tight">Premier Auto Group</div>
                                    <div class="w-8 h-8 rounded-full bg-[var(--color-primary-500)] flex items-center justify-center text-black font-bold">+</div>
                                    <div class="flex items-center gap-2 text-white font-semibold text-xl tracking-tight">
                                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <rect x="3" y="3" width="18" height="18" rx="2" stroke="white" stroke-width="2" fill="none"/>
                                            <path d="M8 12h8M12 8v8" stroke="white" stroke-width="2" stroke-linecap="round"/>
                                        </svg>
                                        CreditApp
                                    </div>
                                </div>
                                <h3 class="text-3xl font-bold text-white mb-4 max-w-md">
                                    How Premier Auto Group increased their approval rate by 35% with CreditApp
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
                                <div class="absolute inset-0 bg-gradient-to-br from-teal-900/40 to-black"></div>
                                <div class="relative z-10 flex justify-between items-end">
                                    <div class="w-12 h-12 rounded-full bg-teal-400/20 blur-xl absolute -left-2 -bottom-2"></div>
                                    <div class="w-10 h-10 rounded-full bg-white/10 backdrop-blur-md border border-white/20 flex items-center justify-center text-white group-hover:bg-white group-hover:text-black transition-colors ml-auto">
                                        <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
                                    </div>
                                </div>
                            </div>
                            <!-- Card 3 -->
                            <div class="bg-[#0A0A0A] rounded-3xl p-8 relative overflow-hidden group h-[240px] flex flex-col justify-end">
                                <div class="absolute inset-0 bg-gradient-to-br from-cyan-900/40 to-black"></div>
                                <div class="relative z-10 flex justify-between items-end">
                                    <div class="w-12 h-12 rounded-full bg-cyan-400/20 blur-xl absolute -left-2 -bottom-2"></div>
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
                    <div class="absolute left-0 top-0 w-64 h-64 bg-teal-500/10 blur-[100px] rounded-full"></div>
                    <div class="absolute right-0 bottom-0 w-64 h-64 bg-cyan-500/10 blur-[100px] rounded-full"></div>
                    
                    <div class="relative z-10 max-w-3xl mx-auto">
                        <h2 class="text-4xl md:text-6xl font-bold text-white mb-6 tracking-tight">
                            Close more deals. <span class="text-[var(--color-primary-500)]">Faster approvals.</span>
                        </h2>
                        <p class="text-gray-400 mb-10">
                            Built specifically for Canadian dealers and finance managers. Get instant access to multiple lenders and competitive rates.
                        </p>
                        <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-md border border-white/10 rounded-full px-4 py-2 text-white text-sm hover:bg-white/20 transition-colors cursor-pointer">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
                            Help Center
                            <kbd class="bg-black/30 px-1.5 py-0.5 rounded text-xs text-gray-400 font-mono">?</kbd>
                        </div>
                    </div>
                </div>

                <!-- Integrations -->
                <div class="text-center mb-32">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
                        Major banks. Credit unions. Alternative lenders.<br>
                        <span class="text-gray-400">Connect with Canada's<br>leading financial institutions.</span>
                    </h2>
                    <button class="bg-gray-100 hover:bg-gray-200 text-black px-6 py-2 rounded-full text-sm font-medium transition-colors flex items-center gap-2 mx-auto mb-16 mt-8">
                        View all lenders
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </button>

                    <div class="grid grid-cols-2 md:grid-cols-4 gap-px bg-gray-200 border border-gray-200 rounded-2xl overflow-hidden">
                        {#each ['TD Bank', 'RBC', 'Scotiabank', 'BMO', 'CIBC', 'Desjardins', 'National Bank', 'Meridian'] as logo}
                        <div class="bg-[#F9FAFB] p-12 flex items-center justify-center grayscale opacity-60 hover:grayscale-0 hover:opacity-100 transition-all duration-300">
                            <span class="font-bold text-xl uppercase tracking-wider">{logo}</span>
                        </div>
                        {/each}
                    </div>
                </div>

                <!-- Blog Section -->
                <div class="mb-12">
                    <h2 class="text-4xl font-bold text-gray-900 mb-12">Insights for Canadian dealers.</h2>
                    <div class="grid md:grid-cols-2 gap-8">
                        <!-- Post 1 -->
                        <div class="group cursor-pointer">
                            <div class="bg-gradient-to-br from-gray-200 to-gray-300 rounded-3xl aspect-[16/9] mb-6 relative overflow-hidden">
                                <div class="absolute inset-0 flex items-center justify-center">
                                    <div class="grid grid-cols-6 gap-4 opacity-50">
                                        {#each Array(24) as _}
                                            <svg class="w-6 h-6 text-teal-600 transform -rotate-45" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 10l7-7m0 0l7 7m-7-7v18"></path></svg>
                                        {/each}
                                    </div>
                                </div>
                            </div>
                            <div class="text-xs font-bold text-gray-500 uppercase tracking-wider mb-2">Dealer Tips</div>
                            <h3 class="text-2xl font-bold text-gray-900 group-hover:text-teal-600 transition-colors">5 ways to improve your credit approval rates in 2024</h3>
                        </div>
                        <!-- Post 2 -->
                        <div class="group cursor-pointer">
                            <div class="bg-gray-100 rounded-3xl aspect-[16/9] mb-6 relative overflow-hidden flex items-center justify-center">
                                <div class="flex gap-4">
                                    <div class="w-16 h-16 rounded-full bg-teal-400 blur-xl opacity-80"></div>
                                    <div class="w-20 h-20 rounded-full bg-cyan-400 blur-xl opacity-80"></div>
                                    <div class="w-12 h-12 rounded-full bg-blue-400 blur-xl opacity-80"></div>
                                </div>
                            </div>
                            <div class="text-xs font-bold text-gray-500 uppercase tracking-wider mb-2">Industry News</div>
                            <h3 class="text-2xl font-bold text-gray-900 group-hover:text-teal-600 transition-colors">Canadian auto lending trends: What dealers need to know</h3>
                        </div>
                    </div>
                </div>


    </main>

    <Footer />
</div>

