<script>
    import { onMount } from 'svelte';

    let isScrolled = false;

    onMount(() => {
        const handleScroll = () => {
            isScrolled = window.scrollY > 20;
        };
        window.addEventListener('scroll', handleScroll);
        return () => window.removeEventListener('scroll', handleScroll);
    });
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
            <a href="#" class="hover:text-white transition-colors">Platform</a>
            <a href="#" class="hover:text-white transition-colors">Solutions</a>
            <a href="#" class="hover:text-white transition-colors">Integrations</a>
            <a href="#" class="hover:text-white transition-colors">Resources</a>
            <a href="#" class="hover:text-white transition-colors">Dealers</a>
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
