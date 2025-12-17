<script lang="ts">
	import { onMount } from 'svelte';

	let scrollY = 0;
</script>

<svelte:window bind:scrollY />

<div class="font-sans text-gray-900 antialiased selection:bg-primary-200 selection:text-primary-900">
	<!-- Hero Section -->
	<section class="relative min-h-screen w-full bg-gradient-to-b from-gray-900 via-gray-800 to-white text-white px-6 md:px-12 lg:px-24 pt-32 pb-24 flex flex-col justify-between">
		<div class="max-w-5xl">
			<div class="mb-6">
				<span class="inline-block px-4 py-2 bg-primary-500/20 border border-primary-500/30 rounded-full text-primary-300 text-sm font-medium">
					Certified StoryBrand Guide Agency
				</span>
			</div>
			<h1 class="font-serif text-5xl md:text-7xl lg:text-8xl leading-[1.1] md:leading-[1.1] tracking-tight">
				Transform confused messaging into customer-winning clarity.
			</h1>
			<p class="mt-8 text-xl md:text-2xl text-gray-300 max-w-3xl">
				We help B2B brands implement the StoryBrand framework with guaranteed 3X ROI—because brands that get their messaging right, grow by winning more customers.
			</p>
		</div>

		<div class="mt-24 flex flex-col sm:flex-row gap-4">
			<a href="#results" class="inline-flex items-center justify-center px-8 py-4 bg-primary-500 hover:bg-primary-600 rounded-full text-base font-semibold text-white transition-colors duration-300">
				See Our Results
			</a>
			<a href="#process" class="inline-flex items-center justify-center px-8 py-4 border border-white/30 rounded-full text-base font-medium hover:bg-white hover:text-gray-900 transition-colors duration-300 backdrop-blur-sm">
				How We Work
			</a>
		</div>
	</section>

	<!-- Trusted Clients -->
	<section class="bg-white px-6 md:px-12 lg:px-24 py-16 md:py-24">
		<p class="text-lg md:text-xl text-gray-600 mb-12">Trusted by 200+ brands globally—from small businesses to multi-million dollar companies</p>
		
		<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-4 md:gap-8">
			<!-- Client logos -->
			{#each ['StructureCraft', 'Tearfund Canada', 'Finzly', 'Organic Traditions', 'Kijiji', 'Pacgeo'] as client}
				<div class="h-20 bg-gray-50 rounded-lg flex items-center justify-center grayscale opacity-70 hover:opacity-100 hover:grayscale-0 transition-all duration-300 border border-gray-100">
					<span class="font-semibold text-gray-700 text-sm text-center px-2">{client}</span>
				</div>
			{/each}
		</div>
	</section>

    <!-- Results Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24" id="results">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 md:mb-24">
            <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900">Proven results that drive real growth</h2>
            <div class="text-gray-600 mt-4 md:mt-0">
                <span class="font-semibold text-primary-600">Guaranteed 3X ROI</span>
            </div>
        </div>

        <div class="space-y-24 md:space-y-32">
            <!-- Case Study 1: Leads at Scale -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Leads at Scale</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Clear StoryBrand messaging transformed their marketing, delivering 285% revenue increase and 30% monthly inbound lead growth for 3 consecutive months.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 bg-primary-50 border border-primary-200 rounded-full text-xs font-medium text-primary-700">+285% Revenue</span>
                        <span class="px-3 py-1 bg-primary-50 border border-primary-200 rounded-full text-xs font-medium text-primary-700">+30% Monthly Leads</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-marketing-team-celebrating-growth-result-1765936279132-3.webp" alt="Leads at Scale Results" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Case Study 2: Veitas Engineers -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Veitas Engineers</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Through strategic StoryBrand messaging and website redesign, Veitas eliminated their competition by clearly communicating their unique value proposition.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">StoryBrand Messaging</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Website Design</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-engineering-firm-team-collaborating-in-m-1765936274412-1.webp" alt="Veitas Engineers" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Case Study 3: HMH Legal -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">HMH Legal</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Started attracting new clients instantly after implementing StoryBrand messaging. Clear communication led to consistent growth and predictable client acquisition.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">StoryBrand Framework</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Website</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Lead Generation</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-legal-professionals-in-consultation-meet-1765936276756-2.webp" alt="HMH Legal" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Case Study 4: StructureCraft -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">StructureCraft</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        North America's leading timber structural engineering-build firm. 3+ year ongoing partnership delivering strategic marketing services and consistent growth.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Strategic Marketing</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Ongoing Partnership</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-timber-construction-project-with-modern--1765936281486-4.webp" alt="StructureCraft" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>
        </div>
        
        <div class="mt-16 text-center">
            <a href="#contact" class="inline-flex items-center justify-center px-8 py-4 bg-gray-900 hover:bg-gray-800 text-white rounded-full text-base font-semibold transition-colors duration-300">
                Get Your Free Marketing Assessment
            </a>
        </div>
    </section>

    <!-- Process Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24" id="process">
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-8 max-w-3xl">Our three-chapter framework for complete StoryBrand transformation</h2>
        <p class="text-xl text-gray-600 mb-16 max-w-2xl">We don't just clarify your message—we build a complete growth engine that turns confusion into customers.</p>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Chapter 1: Messaging -->
            <div class="bg-gray-50 p-8 rounded-xl border border-gray-200 hover:border-primary-300 transition-all duration-300 flex flex-col h-full min-h-[450px]">
                <div class="mb-4">
                    <span class="inline-block px-3 py-1 bg-primary-100 text-primary-700 rounded-full text-xs font-semibold">CHAPTER 1</span>
                </div>
                <h3 class="text-2xl font-bold mb-4">StoryBrand Messaging</h3>
                <p class="text-gray-600 text-base leading-relaxed mb-auto">
                    Clarify what you do using the proven StoryBrand Framework. We examine your brand from every angle to uncover messaging that engages your most important customers.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="/generated/image-marketer-writing-clear-messaging-on-whit-1765936283764-5.webp" alt="StoryBrand Messaging" class="w-full h-full object-cover rounded-lg" />
                </div>
            </div>

            <!-- Chapter 2: Website -->
            <div class="bg-gray-50 p-8 rounded-xl border border-gray-200 hover:border-primary-300 transition-all duration-300 flex flex-col h-full min-h-[450px]">
                <div class="mb-4">
                    <span class="inline-block px-3 py-1 bg-primary-100 text-primary-700 rounded-full text-xs font-semibold">CHAPTER 2</span>
                </div>
                <h3 class="text-2xl font-bold mb-4">StoryBrand Website</h3>
                <p class="text-gray-600 text-base leading-relaxed mb-auto">
                    Custom website designed to capture and convert. We combine compelling copy with strategic design—not just words, not just visuals, but the complete picture.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="/generated/image-web-designer-working-on-laptop-showing-m-1765936286019-6.webp" alt="Website Design" class="w-full h-full object-cover rounded-lg" />
                </div>
            </div>

            <!-- Chapter 3: Marketing -->
            <div class="bg-gray-50 p-8 rounded-xl border border-gray-200 hover:border-primary-300 transition-all duration-300 flex flex-col h-full min-h-[450px]">
                <div class="mb-4">
                    <span class="inline-block px-3 py-1 bg-primary-100 text-primary-700 rounded-full text-xs font-semibold">CHAPTER 3</span>
                </div>
                <h3 class="text-2xl font-bold mb-4">Complete Marketing Strategy</h3>
                <p class="text-gray-600 text-base leading-relaxed mb-auto">
                    Sales funnels and lead generation systems that drive results. From Google Ads to email marketing, we execute the complete strategy with guaranteed ROI.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="/generated/image-marketing-strategist-presenting-campaign-1765936288280-7.webp" alt="Marketing Execution" class="w-full h-full object-cover rounded-lg" />
                </div>
            </div>
        </div>
    </section>

    <!-- Resources Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24">
        <div class="flex flex-col md:flex-row justify-between items-end mb-12">
            <h2 class="font-serif text-3xl md:text-4xl text-gray-900">StoryBrand insights and resources</h2>
            <a href="#newsletter" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                Get free guide <span class="ml-2">→</span>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Resource 1 -->
            <div class="group cursor-pointer">
                <div class="aspect-square bg-gradient-to-br from-primary-600 to-primary-800 rounded-lg overflow-hidden mb-4 relative flex items-center justify-center p-8">
                     <div class="text-white text-center">
                        <div class="text-6xl font-bold mb-4">7</div>
                        <div class="text-xl font-semibold">Website Mistakes</div>
                        <div class="text-sm opacity-90 mt-2">Costing You Business</div>
                     </div>
                </div>
                <h3 class="text-base font-semibold text-gray-900 group-hover:underline">Free PDF: 7 Mistakes on Your Website That Are Costing You Business</h3>
            </div>

             <!-- Resource 2 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-900 rounded-lg overflow-hidden mb-4 relative flex items-center justify-center p-8">
                    <div class="text-white text-center">
                        <div class="text-4xl font-serif mb-4">StoryBrand</div>
                        <div class="text-lg">Framework Guide</div>
                    </div>
                </div>
                <h3 class="text-base font-semibold text-gray-900 group-hover:underline">How to Build the Best StoryBrand Websites</h3>
            </div>

             <!-- Resource 3 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gradient-to-br from-gray-700 to-gray-900 rounded-lg overflow-hidden mb-4 relative flex items-center justify-center p-8">
                     <div class="text-white text-center">
                        <div class="text-3xl font-bold mb-2">ROI</div>
                        <div class="text-xl">Guaranteed</div>
                        <div class="text-6xl font-bold mt-4">3X</div>
                     </div>
                </div>
                <h3 class="text-base font-semibold text-gray-900 group-hover:underline">Why Words Alone Won't Win: The Complete Picture Approach</h3>
            </div>

             <!-- Resource 4 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-primary-100 rounded-lg overflow-hidden mb-4 relative flex items-center justify-center p-8">
                    <div class="text-primary-900 text-center">
                        <div class="text-2xl font-semibold mb-4">StoryBrand Guide</div>
                        <div class="text-lg">vs</div>
                        <div class="text-2xl font-semibold mt-4">Business Made Simple</div>
                    </div>
                </div>
                <h3 class="text-base font-semibold text-gray-900 group-hover:underline">StoryBrand Guide vs Business Made Simple Coach: What's the Difference?</h3>
            </div>

             <!-- Resource 5 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gradient-to-br from-primary-500 to-primary-700 rounded-lg overflow-hidden mb-4 relative flex items-center justify-center p-8">
                    <div class="text-white text-center">
                        <div class="text-4xl mb-4">🤖</div>
                        <div class="text-2xl font-bold">AI + StoryBrand</div>
                        <div class="text-sm mt-4 opacity-90">The Future of Marketing</div>
                    </div>
                </div>
                <h3 class="text-base font-semibold text-gray-900 group-hover:underline">StoryBrand AI Integration: What Won't Change in Marketing</h3>
            </div>

             <!-- Resource 6 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-800 rounded-lg overflow-hidden mb-4 relative flex items-center justify-center p-8">
                     <div class="text-white text-center">
                        <div class="text-5xl font-bold mb-2">200+</div>
                        <div class="text-xl">Brands Transformed</div>
                        <div class="text-sm mt-4 opacity-80">Global Success Stories</div>
                     </div>
                </div>
                <h3 class="text-base font-semibold text-gray-900 group-hover:underline">StoryBrand Website Examples: Real Results from Real Businesses</h3>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="px-6 md:px-12 lg:px-24 py-12" id="newsletter">
        <div class="bg-gradient-to-br from-primary-50 to-primary-100 rounded-2xl p-8 md:p-16 lg:p-20 border border-primary-200">
            <h3 class="font-serif text-2xl md:text-3xl lg:text-4xl text-gray-900 mb-4">Get your free guide: 7 Website Mistakes Costing You Business</h3>
            <p class="text-gray-700 mb-8 max-w-2xl text-lg">Plus monthly StoryBrand insights, marketing strategies, and proven tactics to turn your confused messaging into customer-winning clarity.</p>
            
            <form class="flex flex-col sm:flex-row gap-4 max-w-2xl">
                <input type="email" placeholder="your.email@company.com" class="flex-1 bg-white border border-primary-200 rounded-lg px-5 py-4 text-base placeholder:text-gray-400 focus:ring-2 focus:ring-primary-500 focus:border-primary-500 outline-none" />
                <button type="submit" class="bg-primary-600 hover:bg-primary-700 transition-colors text-white px-8 py-4 rounded-lg text-base font-semibold whitespace-nowrap">
                    Get Free Guide
                </button>
            </form>
            <p class="text-xs text-gray-600 mt-4">We respect your privacy. No spam, ever. Unsubscribe anytime. By signing up, you agree to receive communications from Creativeo.</p>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="relative bg-gradient-to-b from-gray-800 via-gray-900 to-black pt-32 pb-48 px-6 md:px-12 lg:px-24 overflow-hidden" id="contact">
        <div class="max-w-5xl relative z-10">
            <div class="mb-6">
                <span class="inline-block px-4 py-2 bg-primary-500/20 border border-primary-500/30 rounded-full text-primary-300 text-sm font-medium">
                    Certified StoryBrand Guides • Guaranteed 3X ROI
                </span>
            </div>
            <h2 class="font-serif text-4xl md:text-6xl lg:text-7xl text-white leading-tight mb-8">
                Ready to transform your confused messaging into customer-winning clarity?
            </h2>
            <p class="text-xl md:text-2xl text-gray-300 mb-12 max-w-3xl">
                We only work with businesses we can deliver 3X ROI minimum. Let's see if we're the right fit for your complete StoryBrand transformation.
            </p>
            
            <div class="mt-16 flex flex-col sm:flex-row gap-4">
                 <a href="#" class="inline-flex items-center justify-center px-8 py-4 bg-primary-500 hover:bg-primary-600 rounded-full text-lg font-semibold text-white transition-colors duration-300">
                    Schedule Free Consultation
                </a>
                <a href="#newsletter" class="inline-flex items-center justify-center px-8 py-4 border border-white/30 rounded-full text-lg font-medium text-white hover:bg-white hover:text-gray-900 transition-colors duration-300 backdrop-blur-sm">
                    Download Free Guide
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 px-6 md:px-12 lg:px-24 pt-24 pb-12 relative overflow-hidden">
        <div class="relative z-10">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mb-24">
                <div class="col-span-1 md:col-span-2">
                    <div class="mb-8">
                        <!-- Logo -->
                        <svg width="40" height="40" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="text-primary-500">
                            <path
                                fill-rule="evenodd"
                                clip-rule="evenodd"
                                d="M5.0473 17.8386L5.69453 18.9586V18.9601H18.3003L18.9314 17.84H6.34063L6.82626 16.9993H19.4308L20.078 15.8807H7.47237L7.95715 15.0414H16.0358L16.0366 15.0429L16.0375 15.0414H20.5603L20.5612 15.0429L21.2084 13.9228L21.208 13.922L21.2084 13.9213H21.2075L14.9084 3.00677L14.9106 3.00296L14.9062 3.00296L13.6177 3.00296L5.0473 17.8386ZM14.261 4.12767L13.7751 4.96887L18.9438 13.9213H19.9139L14.261 4.12767ZM13.1286 6.08808L12.6467 6.9225L16.6749 13.9006L16.6634 13.9213H17.6511L13.1286 6.08808ZM11.9999 8.04225L8.60411 13.9213H15.3899L11.9999 8.04225ZM6.99833 3.30006C7.33866 3.10343 7.7248 2.99993 8.11786 3L2.30033 13.0776C2.10357 12.7371 2 12.3508 2 11.9575C2 11.5643 2.10357 11.178 2.30033 10.8375L6.17916 4.12006C6.37543 3.77951 6.65798 3.49669 6.99833 3.30006ZM9.08869 3H10.3816L3.43223 15.0384L2.785 13.9184L9.08869 3ZM11.3509 3H12.6424L4.56262 16.9963L3.91691 15.8777L11.3509 3ZM21.7064 13.0598C21.8988 12.7254 22 12.3463 22 11.9605C22 11.5746 21.8988 11.1956 21.7064 10.8611L17.8039 4.10233C17.6108 3.7681 17.3331 3.49057 16.9987 3.2976C16.6644 3.10463 16.2852 3.00302 15.8992 3.00296H15.8741L21.6931 13.082L21.7064 13.0598ZM17.7995 19.7994H6.17916C6.37472 20.1412 6.65692 20.4253 6.99728 20.6232C7.33763 20.8212 7.72414 20.9258 8.11786 20.9269H15.8829C16.2737 20.9261 16.6572 20.8212 16.994 20.6231C17.3309 20.4249 17.6089 20.1406 17.7995 19.7994Z"
                                fill="currentColor"
                            />
                        </svg>
                    </div>
                    <h3 class="text-2xl font-serif text-white mb-4">Creativeo</h3>
                    <p class="text-gray-400 mb-6 max-w-md">
                        Certified StoryBrand Guide agency helping B2B brands transform confused messaging into customer-winning clarity with guaranteed 3X ROI.
                    </p>
                    <a href="#contact" class="inline-flex items-center text-primary-400 hover:text-primary-300 transition-colors font-medium">
                        Work with us <span class="ml-2">→</span>
                    </a>
                </div>
                
                <div class="space-y-4">
                    <h4 class="font-semibold text-white text-lg">Toronto, Canada</h4>
                    <div class="pt-2 text-sm space-y-2">
                        <p><a href="mailto:hello@creativeo.com" class="hover:text-white transition-colors">hello@creativeo.com</a></p>
                        <p class="text-gray-500 text-xs mt-4">Serving clients globally across North America, Europe, and Asia</p>
                    </div>
                    <div class="pt-6">
                        <h5 class="font-medium text-white mb-3">Certifications</h5>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1 bg-gray-800 text-gray-300 rounded text-xs">StoryBrand Certified</span>
                            <span class="px-3 py-1 bg-gray-800 text-gray-300 rounded text-xs">HubSpot Partner</span>
                            <span class="px-3 py-1 bg-gray-800 text-gray-300 rounded text-xs">Google Partner</span>
                        </div>
                    </div>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between items-center border-t border-gray-800 pt-8 gap-4">
                <div class="flex gap-6 text-sm">
                    <a href="#" class="hover:text-white transition-colors">LinkedIn</a>
                    <a href="#" class="hover:text-white transition-colors">Twitter</a>
                    <a href="#" class="hover:text-white transition-colors">Facebook</a>
                </div>
                
                <div class="flex gap-6 text-xs text-gray-500">
                    <a href="#" class="hover:text-gray-300 transition-colors">Privacy Policy</a>
                    <a href="#" class="hover:text-gray-300 transition-colors">Terms of Service</a>
                </div>
            </div>

            <div class="text-center text-xs text-gray-600 mt-8">
                <p>© 2025 Creativeo. All rights reserved.</p>
            </div>
        </div>
    </footer>
</div>

<style>
    /* Custom utility for vertical writing mode */
    .writing-vertical-rl {
        writing-mode: vertical-rl;
    }
</style>

