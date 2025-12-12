<script lang="ts">
    import { onMount } from 'svelte';

    let isScrolled = $state(false);
    let isDealersOpen = $state(false);
    let dropdownRef: HTMLDivElement | null = $state(null);

    onMount(() => {
        const handleScroll = () => {
            isScrolled = window.scrollY > 20;
        };
        window.addEventListener('scroll', handleScroll);
        return () => window.removeEventListener('scroll', handleScroll);
    });

    // Close dropdown when clicking outside
    $effect(() => {
        const handleClickOutside = (event: MouseEvent) => {
            if (dropdownRef && !dropdownRef.contains(event.target as Node)) {
                isDealersOpen = false;
            }
        };

        if (isDealersOpen) {
            document.addEventListener('click', handleClickOutside);
            return () => document.removeEventListener('click', handleClickOutside);
        }
    });

    function toggleDealers(event: MouseEvent) {
        event.stopPropagation();
        isDealersOpen = !isDealersOpen;
    }
</script>

<nav class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 {isScrolled ? 'bg-black/80 backdrop-blur-md py-4' : 'bg-transparent py-6'}">
    <div class="container mx-auto px-6 flex items-center justify-between">
        <!-- Logo -->
        <a href="/" class="flex items-center gap-2 text-white font-semibold text-xl tracking-tight">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect x="3" y="3" width="18" height="18" rx="2" stroke="white" stroke-width="2" fill="none"/>
                <path d="M8 12h8M12 8v8" stroke="white" stroke-width="2" stroke-linecap="round"/>
            </svg>
            CreditApp
        </a>

        <!-- Links -->
        <div class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-300">
            <!-- Dealers Dropdown -->
            <div class="relative" bind:this={dropdownRef}>
                <button 
                    onclick={toggleDealers}
                    class={[
                        'flex items-center gap-1 hover:text-white transition-colors',
                        isDealersOpen ? 'text-white' : ''
                    ]}
                >
                    Dealers
                    <svg 
                        width="16" 
                        height="16" 
                        viewBox="0 0 24 24" 
                        fill="none" 
                        stroke="currentColor" 
                        stroke-width="2" 
                        stroke-linecap="round" 
                        stroke-linejoin="round"
                        class={[
                            'transition-transform duration-200',
                            isDealersOpen ? 'rotate-180' : ''
                        ]}
                    >
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </button>
                
                {#if isDealersOpen}
                    <div class="absolute top-full left-0 mt-2 w-56 bg-black/95 backdrop-blur-md border border-gray-800 rounded-lg shadow-xl overflow-hidden">
                        <a href="#" class="block px-4 py-3 text-gray-300 hover:text-white hover:bg-white/5 transition-colors">
                            Dealer Tools
                        </a>
                        <a href="#" class="block px-4 py-3 text-gray-300 hover:text-white hover:bg-white/5 transition-colors">
                            DealFlow
                        </a>
                        <a href="#" class="block px-4 py-3 text-gray-300 hover:text-white hover:bg-white/5 transition-colors">
                            ID & Income Verification
                        </a>
                    </div>
                {/if}
            </div>
            
            <a href="#" class="hover:text-white transition-colors">Solutions</a>
            <a href="#" class="hover:text-white transition-colors">Integrations</a>
            <a href="#" class="hover:text-white transition-colors">Resources</a>
        </div>

        <!-- CTA -->
        <a href="#" class="hidden md:flex items-center gap-1 text-sm font-medium text-white hover:text-[var(--color-primary-500)] transition-colors">
            Request Demo
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <path d="M5 12h14M12 5l7 7-7 7"/>
            </svg>
        </a>
        
        <!-- Mobile Menu Button -->
        <button class="md:hidden text-white">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <line x1="3" y1="12" x2="21" y2="12"></line>
                <line x1="3" y1="6" x2="21" y2="6"></line>
                <line x1="3" y1="18" x2="21" y2="18"></line>
            </svg>
        </button>
    </div>
</nav>
