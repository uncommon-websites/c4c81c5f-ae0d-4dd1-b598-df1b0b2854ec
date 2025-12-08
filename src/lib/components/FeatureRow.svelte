<script lang="ts">
    export let title: string;
    export let description: string;
    export let image: string;
    export let icon: string;

    // Extract the bold part of the description (first sentence)
    $: splitDesc = description.split('. ');
    $: boldDesc = splitDesc[0] + '.';
    $: restDesc = splitDesc.slice(1).join('. ');
</script>

<div class="bg-[#F3F4F6] rounded-3xl p-8 md:p-12 transition-all hover:bg-gray-200 group">
    <!-- Header -->
    <div class="flex items-center gap-3 mb-8">
        <div class="text-blue-600">
            {#if icon === 'lock'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>
            {:else if icon === 'connect'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="9" cy="7" r="4"></circle><path d="M23 21v-2a4 4 0 0 0-3-3.87"></path><path d="M16 3.13a4 4 0 0 1 0 7.75"></path></svg>
            {:else if icon === 'data'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"></path><polyline points="3.27 6.96 12 12.01 20.73 6.96"></polyline><line x1="12" y1="22.08" x2="12" y2="12"></line></svg>
            {:else if icon === 'lab'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M6 14h12l-3.9-6.8a2 2 0 0 0-3.5 0L6 14z"></path><path d="M2 22h20"></path><path d="M10 14v4"></path><path d="M14 14v4"></path></svg>
            {:else if icon === 'preview'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
            {:else if icon === 'guard'}
                <svg class="w-6 h-6" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path></svg>
            {/if}
        </div>
        <h3 class="text-xl font-semibold text-gray-900">{title}</h3>
    </div>

    <!-- Image Placeholder / Abstract UI -->
    <div class="bg-white rounded-xl shadow-sm border border-gray-200 overflow-hidden mb-8 aspect-[16/9] relative group-hover:shadow-md transition-shadow">
        {#if image === 'collateral'}
            <!-- Collateral UI -->
            <div class="p-6 h-full flex flex-col">
                <div class="flex justify-between items-center mb-6 border-b border-gray-100 pb-4">
                    <div class="font-bold text-gray-800">Collateral</div>
                    <div class="flex gap-2">
                        <div class="w-20 h-8 bg-gray-100 rounded"></div>
                    </div>
                </div>
                <div class="space-y-3">
                    <div class="flex justify-between text-xs text-gray-400 uppercase tracking-wider">
                        <span>Collateral Type</span>
                        <span>Value</span>
                        <span>Status</span>
                    </div>
                    {#each [1, 2, 3] as i}
                    <div class="flex justify-between items-center py-2 border-b border-gray-50">
                        <div class="w-24 h-4 bg-gray-100 rounded"></div>
                        <div class="w-16 h-4 bg-gray-100 rounded"></div>
                        <div class="w-12 h-4 bg-green-100 text-green-600 rounded-full text-[10px] flex items-center justify-center">Active</div>
                    </div>
                    {/each}
                </div>
            </div>
        {:else if image === 'connect'}
            <!-- Connect UI -->
            <div class="p-6 h-full flex flex-col items-center justify-center bg-gray-50">
                <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-200 w-3/4">
                    <div class="flex items-center gap-3 mb-4">
                        <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center text-blue-600">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path></svg>
                        </div>
                        <div class="text-sm font-medium">Payment Received Webhook</div>
                    </div>
                    <div class="h-px bg-gray-100 w-full mb-4"></div>
                    <div class="flex justify-center">
                        <div class="bg-gray-100 text-gray-500 text-xs px-2 py-1 rounded">Branch on due date</div>
                    </div>
                </div>
            </div>
        {:else if image === 'data'}
            <!-- Data UI -->
            <div class="p-6 h-full flex flex-col">
                <div class="flex gap-4 mb-6">
                    <div class="w-1/2 p-4 bg-gray-50 rounded-lg border border-gray-100">
                        <div class="text-xs text-gray-400 mb-1">Avg. min. pay cents</div>
                        <div class="text-xl font-bold text-gray-900">333.33</div>
                        <div class="mt-4 h-16 flex items-end gap-1">
                            {#each [40, 60, 30, 70, 50, 80] as h}
                                <div class="w-full bg-blue-200 rounded-t" style="height: {h}%"></div>
                            {/each}
                        </div>
                    </div>
                    <div class="w-1/2 p-4 bg-gray-50 rounded-lg border border-gray-100">
                        <div class="text-xs text-gray-400 mb-1">Average balance</div>
                        <div class="text-xl font-bold text-gray-900">$3,183.48</div>
                         <div class="mt-4 h-2 bg-gray-200 rounded-full overflow-hidden">
                            <div class="h-full bg-blue-500 w-2/3"></div>
                        </div>
                    </div>
                </div>
            </div>
        {:else if image === 'lab'}
            <!-- Lab UI -->
            <div class="p-6 h-full bg-white">
                <div class="font-mono text-xs text-gray-400 mb-4">Action Timeline</div>
                <div class="space-y-4 relative pl-4 border-l border-gray-200">
                    <div class="relative">
                        <div class="absolute -left-[21px] top-1 w-3 h-3 rounded-full bg-green-500 border-2 border-white"></div>
                        <div class="text-xs font-medium text-gray-900">Cycle 1: Dec 13 12:43PM - 15 Dec @ 00:00AM</div>
                        <div class="mt-1 text-xs text-gray-500 pl-2 border-l border-gray-100 ml-1">Automation: Account Created</div>
                    </div>
                     <div class="relative">
                        <div class="absolute -left-[21px] top-1 w-3 h-3 rounded-full bg-green-500 border-2 border-white"></div>
                        <div class="text-xs font-medium text-gray-900">Minimum Payment</div>
                         <div class="mt-1 text-xs text-gray-500 pl-2 border-l border-gray-100 ml-1">Automation: Generate Statement</div>
                    </div>
                </div>
            </div>
        {:else if image === 'preview'}
            <!-- Preview UI -->
            <div class="p-6 h-full">
                <table class="w-full text-xs">
                    <thead>
                        <tr class="text-gray-400 border-b border-gray-100">
                            <th class="text-left pb-2 font-normal">Action</th>
                            <th class="text-right pb-2 font-normal">Current</th>
                            <th class="text-right pb-2 font-normal">Preview</th>
                        </tr>
                    </thead>
                    <tbody class="text-gray-600">
                        <tr class="border-b border-gray-50">
                            <td class="py-2">Account Status</td>
                            <td class="py-2 text-right text-red-500">Suspended</td>
                            <td class="py-2 text-right text-green-500">Active</td>
                        </tr>
                         <tr class="border-b border-gray-50">
                            <td class="py-2">Minimum Payment</td>
                            <td class="py-2 text-right">$2,950.00</td>
                            <td class="py-2 text-right">$0.00</td>
                        </tr>
                         <tr>
                            <td class="py-2">Total Balance</td>
                            <td class="py-2 text-right">$5,925.00</td>
                            <td class="py-2 text-right">$2,975.00</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        {:else if image === 'guard'}
            <!-- Guard UI -->
            <div class="p-6 h-full flex flex-col justify-center">
                <div class="text-xs text-gray-400 mb-2">Customer ID: 42784724728</div>
                <div class="grid grid-cols-2 gap-4">
                    <div class="p-3 bg-green-50 rounded border border-green-100">
                        <div class="text-[10px] text-green-600 uppercase">Account status</div>
                        <div class="text-sm font-bold text-green-700">Active</div>
                    </div>
                    <div class="p-3 bg-red-50 rounded border border-red-100">
                        <div class="text-[10px] text-red-600 uppercase">Account substatus</div>
                        <div class="text-sm font-bold text-red-700">Delinquent</div>
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4 mt-4">
                    <div>
                        <div class="text-[10px] text-gray-400 uppercase">Missed payments</div>
                        <div class="text-lg font-bold">3</div>
                    </div>
                     <div>
                        <div class="text-[10px] text-gray-400 uppercase">Payment frequency</div>
                        <div class="text-lg font-bold">1</div>
                    </div>
                </div>
            </div>
        {/if}
    </div>

    <!-- Footer -->
    <div class="flex items-end justify-between gap-4">
        <div class="max-w-xl">
            <p class="text-gray-900 text-lg leading-relaxed">
                <span class="font-bold">{boldDesc}</span> <span class="text-gray-600">{restDesc}</span>
            </p>
        </div>
        <button class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center text-gray-600 hover:bg-black hover:text-white hover:border-black transition-colors flex-shrink-0">
            <svg class="w-4 h-4" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <line x1="7" y1="17" x2="17" y2="7"></line>
                <polyline points="7 7 17 7 17 17"></polyline>
            </svg>
        </button>
    </div>
</div>
