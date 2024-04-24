<script>
    import btnMenu from '../assets/menu.png'
    import heroBlog from '../assets/blogHero.jpeg'
    import mainBlog from '../assets/mainBlog.jpeg'
    import recent2 from '../assets/recent2.jpeg'
    import recent3 from '../assets/recent3.jpeg'
    import recent4 from '../assets/recent4.jpeg'

    let isMobile = false

    const toggleMenuContent = () => isMobile = !isMobile
</script>

<div class="font-ralewayRegular">

    <nav class="bg-white lg:py-[1.31rem] md:py-[0.9rem] py-[1.31rem] border">
        <div class="container mx-auto flex justify-between items-center lg:px-0 px-6">
            <button class="flex items-center lg:gap-[0.94rem] gap-[0.68rem] logo">
                <svg class="lg:w-[44px] lg:h-[44px] w-[32px] h-[32px]" width="44" height="44" viewBox="0 0 44 44" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M4.88945 38.9723C1.09221 35.2276 -0.689229 29.5324 0.381427 24.2982C1.44056 18.4198 6.00621 13.2958 11.7719 11.6808C14.5945 14.5445 17.453 17.3696 20.2885 20.2179C20.8725 20.7814 21.4078 21.3949 22.0379 21.9084C20.0285 21.9289 18.0152 21.8546 16.0084 21.9327C13.2357 22.1082 10.8869 24.7234 11.0419 27.5037C11.0163 30.3097 13.5328 32.8455 16.3401 32.8288C21.8624 32.8417 27.3835 32.8276 32.9033 32.8378C36.5314 36.4698 40.1532 40.1096 43.8006 43.7237C43.2371 43.8312 42.6647 43.8018 42.096 43.7967C33.5807 43.798 25.068 43.7967 16.5553 43.798C12.238 43.8095 7.92469 42.0575 4.88945 38.9723Z" fill="#7C4EE4"/><path d="M10.7578 10.713C7.16802 7.14752 3.63331 3.52317 -1.40422e-06 -3.8147e-06C8.49865 0.0332943 16.996 0.00511477 25.4947 0.0153607C26.9214 0.0345714 28.3621 -0.0653203 29.7722 0.202346C33.3863 0.700533 36.8096 2.46916 39.3108 5.12275C42.0911 8.00558 43.7176 11.9475 43.8444 15.9459C43.9392 19.2411 43.0068 22.5619 41.2228 25.3333C39.1238 28.5568 35.8798 31.1054 32.1479 32.1248C29.3611 29.2932 26.5308 26.5013 23.726 23.6851C23.1613 23.1613 22.6874 22.5337 22.0394 22.1008C22.1495 22.0099 22.2686 21.9331 22.3993 21.8716C24.1807 21.9087 25.966 21.9036 27.7487 21.8806C30.515 21.8037 32.9432 19.2756 32.8881 16.5055C32.9688 14.2553 31.446 12.0935 29.347 11.3213C28.5466 10.9755 27.6629 10.9704 26.8061 10.9781C21.6347 10.9832 16.4645 10.9768 11.2944 10.9819C11.078 10.9832 10.8987 10.8935 10.7578 10.713Z" fill="#7C4EE4"/></svg>
                <span class="text-[#333] lg:text-[2.106rem] font-ralewayExtraBold leading-[normal] text-[1.51213rem]">Zarrin</span>
            </button>
            <div class="md:flex items-center gap-[2.62rem] hidden">
                <div class="flex items-center gap-[3.62rem]">
                    <button class="text-[#7C4EE4] lg:text-base text-[0.718rem] font-ralewayMedium leading-[150%]">Blog</button>
                    <button class="text-[#333] lg:text-base text-[0.718rem] font-ralewayMedium leading-[150%]">About</button>
                </div>
                <div class="flex items-center gap-9">
                    <button>
                        <svg class="lg:w-[23px] lg:h-[23px] w-[17px] h-[17px]" width="23" height="23" viewBox="0 0 23 23" fill="none" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" clip-rule="evenodd" d="M16.864 2.74285C20.7917 6.46981 21.0348 12.6476 17.4121 16.6716L21.9172 21.1619C22.1157 21.3673 22.1128 21.6939 21.9108 21.8959C21.7089 22.0979 21.3823 22.1007 21.1768 21.9023L16.6716 17.4121C12.6476 21.0348 6.46981 20.7917 2.74285 16.864C-0.984114 12.9363 -0.903063 6.75424 2.92559 2.92559C6.75424 -0.903063 12.9363 -0.984114 16.864 2.74285ZM1.125 10.028C1.125 14.9444 5.11048 18.9299 10.0268 18.9299C14.9408 18.9241 18.9229 14.942 18.9286 10.028C18.9286 5.1117 14.9432 1.12622 10.0268 1.12622C5.11048 1.12622 1.125 5.1117 1.125 10.028Z" fill="#333333"/></svg>
                    </button>
                    <button class="lg:py-4 py-[0.72rem] lg:text-base text-[0.718rem] lg:px-12 px-[2.15rem] bg-[#7C4EE4] rounded-lg text-white font-ralewaySemiBold leading-[150%]">Contact Us</button>
                </div>
            </div>
            <button class="md:hidden {isMobile ? 'hidden' : ''}" on:click={toggleMenuContent}>
                <img src="{btnMenu}" class="w-[2.125rem] h-[2.125rem]" alt="">
            </button>
            <div class="{isMobile ? 'translate-x-0 transition-transform duration-[200ms] ease-linear' : ' translate-x-[1000px] translate-y-0 transition-transform duration-[0.2s] ease-[ease-in]'} fixed inset-0 w-full h-screen bg-white flex flex-col gap-20 md:hidden">
                <div class="flex justify-between items-center px-6 py-[1.31rem] bg-white border-b border-[#EAEAEA]">
                    <div class="flex items-center lg:gap-[0.94rem] gap-[0.68rem] logo">
                        <svg class="lg:w-[44px] lg:h-[44px] w-[32px] h-[32px]" width="44" height="44" viewBox="0 0 44 44" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M4.88945 38.9723C1.09221 35.2276 -0.689229 29.5324 0.381427 24.2982C1.44056 18.4198 6.00621 13.2958 11.7719 11.6808C14.5945 14.5445 17.453 17.3696 20.2885 20.2179C20.8725 20.7814 21.4078 21.3949 22.0379 21.9084C20.0285 21.9289 18.0152 21.8546 16.0084 21.9327C13.2357 22.1082 10.8869 24.7234 11.0419 27.5037C11.0163 30.3097 13.5328 32.8455 16.3401 32.8288C21.8624 32.8417 27.3835 32.8276 32.9033 32.8378C36.5314 36.4698 40.1532 40.1096 43.8006 43.7237C43.2371 43.8312 42.6647 43.8018 42.096 43.7967C33.5807 43.798 25.068 43.7967 16.5553 43.798C12.238 43.8095 7.92469 42.0575 4.88945 38.9723Z" fill="#7C4EE4"/><path d="M10.7578 10.713C7.16802 7.14752 3.63331 3.52317 -1.40422e-06 -3.8147e-06C8.49865 0.0332943 16.996 0.00511477 25.4947 0.0153607C26.9214 0.0345714 28.3621 -0.0653203 29.7722 0.202346C33.3863 0.700533 36.8096 2.46916 39.3108 5.12275C42.0911 8.00558 43.7176 11.9475 43.8444 15.9459C43.9392 19.2411 43.0068 22.5619 41.2228 25.3333C39.1238 28.5568 35.8798 31.1054 32.1479 32.1248C29.3611 29.2932 26.5308 26.5013 23.726 23.6851C23.1613 23.1613 22.6874 22.5337 22.0394 22.1008C22.1495 22.0099 22.2686 21.9331 22.3993 21.8716C24.1807 21.9087 25.966 21.9036 27.7487 21.8806C30.515 21.8037 32.9432 19.2756 32.8881 16.5055C32.9688 14.2553 31.446 12.0935 29.347 11.3213C28.5466 10.9755 27.6629 10.9704 26.8061 10.9781C21.6347 10.9832 16.4645 10.9768 11.2944 10.9819C11.078 10.9832 10.8987 10.8935 10.7578 10.713Z" fill="#7C4EE4"/></svg>
                        <span class="text-[#333] lg:text-[2.106rem] font-ralewayExtraBold leading-[normal] text-[1.51213rem]">Zarrin</span>
                    </div>
                    <button on:click={toggleMenuContent}>
                        <svg width="24" height="25" viewBox="0 0 24 25" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M18 6.5L6 18.5M6 6.5L18 18.5" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
                    </button>
                </div>
                <div class="px-6 mt-5 flex flex-col items-center gap-3">
                    <button class="text-[#333] p-3 text-[0.875rem] font-ralewayMedium leading-[150%]">Blog</button>
                    <button class="text-[#333] p-3 text-[0.875rem] font-ralewayMedium leading-[150%]">About</button>
                    <button class="py-[0.72rem] text-[0.718rem] px-[2.15rem] bg-[#7C4EE4] rounded-lg text-white font-ralewaySemiBold leading-[150%]">Contact Us</button>
                </div>
            </div>
        </div>
    </nav>
    
    <section class="hero lg:min-h-[49.75rem] md:h-[35.72188rem] min-h-[47.875rem] md:pb-0 pb-[2.62rem] bg-[#7C4EE4] flex items-center lg:mb-[8.31rem] md:mb-[5.88rem] mb-[2.62rem]">
        <div class="container mx-auto flex justify-between items-start md:flex-row flex-col lg:px-0 px-6 md:mt-0 mt-[2.56rem] lg:gap-0 md:gap-[2.06rem] gap-[3.63rem]">
            <div class="flex flex-col items-start max-w-[36.25rem]">
                <h4 class="text-white lg:mb-[2.31rem] md:mb-[1.67rem] mb-[0.37rem] lg:text-base text-[0.718rem] font-ralewayBold leading-[150%] tracking-[0.1rem]">Featured Post</h4>
                <h1 class="text-white lg:text-[4rem] md:text-[2.87213rem] text-[2.25rem] lg:mb-7 md:mb-[1.23rem] mb-[1.19rem] font-ralewayBold lg:leading-[5.375rem] md:leading-[3.85938rem] leading-[2.51563rem]">How AI will Change the Future</h1>
                <p class="text-white max-w-[26rem] lg:text-base text-[0.718rem] lg:mb-16 md:mb-[2.92rem] mb-[1.63rem] leading-[150%]">The future of AI will see home robots having enhanced intelligence, increased capabilities, and becoming more personal and possibly cute. For example, home robots will overcome navigation, direction</p>
                <button class="lg:py-4 py-[0.72rem] lg:px-12 px-[2.15rem] bg-white rounded-lg text-[#373737] lg:text-sm text-[0.62825rem] font-ralewayBold leading-[150%]">Read more</button>
            </div>
            <img src="{heroBlog}" alt="hero" class="w-full lg:max-w-[38rem] md:max-w-[27.28rem] lg:h-[36rem] md:h-[25rem] h-[20.625rem] object-cover rounded-2xl">
        </div>
    </section>

    <section id="main-blog" class="container mx-auto lg:px-0 px-6 flex flex-col lg:items-end items-start lg:-space-y-60 lg:mb-[5.06rem] md:mb-[3.64rem]">
        <img src="{mainBlog}" class="lg:h-[36rem] md:h-[18.849rem] h-[12.51rem] w-full object-cover rounded-2xl" alt="">
        <div class="bg-white rounded-2xl max-w-[57.5rem] lg:p-8 lg:pt-8 pt-[1.67rem] lg:pb-[2.63rem] pb-[1.77rem] lg:pr-[6.5rem]">
            <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">16 March 2023</span>
            </div>
            <h4 class="text-[#333] lg:text-[2rem] text-[1.43606rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] tracking-[-0.0625rem]">How to make a Game look more attractive with New VR & AI Technology</h4>
            <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Google has been investing in AI for many years and bringing its benefits to individuals, businesses and communities. Whether it’s publishing state-of-the-art research, building helpful products or developing tools and resources that enable others, we’re committed to making AI accessible to everyone.</h5>
            <button class="lg:py-4 py-[0.72rem] lg:px-12 px-[2.15rem] border rounded-lg border-solid border-[#7C4EE4] text-[#7C4EE4] lg:text-sm text-[0.62825rem] font-ralewayBold leading-[150%]">Read More</button>
        </div>
    </section>

    <section id="recent-posts" class="container mx-auto lg:px-0 px-6 flex flex-col lg:items-start mb-[6.12rem]">
        <div class="flex justify-between items-center w-full lg:mb-[5.06rem] mb-[3.64rem]">
            <h2 class="text-[#333] lg:text-5xl md:text-[2.15406rem] text-xl font-ralewayBold lg:leading-[3.125rem] leading-[2.24381rem] tracking-[-0.055rem]">Our Recent Post</h2>
            <button class="bg-[#7C4EE4] rounded-lg lg:px-12 px-[2.15rem] lg:py-4 py-[0.72rem] text-white lg:text-sm text-[0.62825rem] font-ralewayBold leading-[150%]">View All</button>
        </div>
        <div class="grid lg:grid-cols-3 sm:grid-cols-2 lg:gap-y-[3.94rem] gap-[2.18rem] gap-x-4">
            <div class="flex lg:col-span-3 sm:col-span-2 justify-between lg:flex-nowrap flex-wrap items-start gap-[3.5rem]">
                <img src="{mainBlog}" class="lg:w-[44.5rem] md:max-w-[31.95225rem] w-full object-cover rounded-2xl lg:max-h-[28.5rem] md:max-h-[20.46381rem]" alt="">
                <div class="max-w-[29rem] lg:mt-4">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">16 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] text-[1.43606rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] tracking-[-0.0625rem]">How to make a Game look more attractive with New VR & AI Technology</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem]">Google has been investing in AI for many years and bringing its benefits to individuals, businesses and communities. Whether it’s publishing state-of-the-art research, building helpful products or developing tools and resources that enable others, we’re committed to making AI accessible to everyone.</h5>
                    <button class="lg:py-4 py-[0.72rem] lg:px-12 px-[2.15rem] border rounded-lg border-solid border-[#7C4EE4] text-[#7C4EE4] lg:text-sm text-[0.62825rem] font-ralewayBold leading-[150%]">Read More</button>
                </div>
            </div>
            <div class="flex flex-col">
                <img src="{recent2}" class="max-w-[25rem] h-full w-full md:max-h-[22.5rem] max-h-[16.15563rem] object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">Travel</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">13 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] tracking-[-0.0625rem]">8 Rules of Travelling In Sea You Need To Know</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Travelling in sea has many advantages. Some of the advantages of transporting goods by sea include: you can ship large volumes at costs </h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
            <div class="flex flex-col">
                <img src="{recent3}" class="max-w-[25rem] h-full w-full md:min-h-[22.5rem] min-h-[16.15563rem] object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">11 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] tracking-[-0.0625rem]">How to build strong portfolio and get a Job in UI/UX</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from</h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
            <div class="flex flex-col">
                <img src="{recent4}" class="max-w-[25rem] h-full w-full md:max-h-[22.5rem] max-h-[16.15563rem] object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">Sports</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">10 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] tracking-[-0.0625rem]">How to Be a Professional Footballer in 2023</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment. survival strategies to ensure proactive </h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
        </div>
    </section>

    <section id="popular-posts" class="container mx-auto flex flex-col items-start lg:mb-[11.94rem] mb-[6rem] lg:px-0 px-6">
        <div class="flex justify-between items-center w-full lg:mb-[5.06rem] mb-[2.81rem]">
            <h2 class="text-[#333] lg:text-5xl md:text-[2.15406rem] text-xl font-ralewayBold lg:leading-[3.125rem] leading-[2.24381rem] tracking-[-0.055rem]">Popular Post</h2>
            <button class="bg-[#7C4EE4] rounded-lg lg:px-12 px-[2.15rem] lg:py-4 py-[0.72rem] text-white lg:text-sm text-[0.62825rem] font-ralewayBold leading-[150%]">View All</button>
        </div>
        <div class="grid lg:grid-cols-3 md:grid-cols-2 gap-y-[3.94rem] gap-x-4">
            <div class="flex flex-col">
                <img src="{recent2}" class="max-w-[25rem] w-full md:h-[22.5rem] h-[16.15563rem]  object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">11 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] md:tracking-[-0.0625rem]">How to build strong portfolio and get a Job in UI/UX</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from</h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
            <div class="flex flex-col">
                <img src="{recent3}" class="max-w-[25rem] w-full md:h-[22.5rem] h-[16.15563rem] object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">11 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] md:tracking-[-0.0625rem]">How to build strong portfolio and get a Job in UI/UX</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from</h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
            <div class="flex flex-col">
                <img src="{recent4}" class="max-w-[25rem] w-full md:h-[22.5rem] h-[16.15563rem] object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">11 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] md:tracking-[-0.0625rem]">How to build strong portfolio and get a Job in UI/UX</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from</h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
            <div class="flex flex-col">
                <img src="{recent2}" class="max-w-[25rem] w-full md:h-[22.5rem] h-[16.15563rem] object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">11 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] md:tracking-[-0.0625rem]">How to build strong portfolio and get a Job in UI/UX</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from</h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
            <div class="flex flex-col">
                <img src="{recent3}" class="max-w-[25rem] w-full md:h-[22.5rem] h-[16.15563rem] object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">11 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] md:tracking-[-0.0625rem]">How to build strong portfolio and get a Job in UI/UX</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from</h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
            <div class="flex flex-col">
                <img src="{recent4}" class="max-w-[25rem] w-full md:h-[22.5rem] h-[16.15563rem] object-cover rounded-2xl" alt="">
                <div class="mt-10">
                    <div class="flex gap-2 items-center lg:mb-[1.56rem] mb-[1.13rem]">
                        <span class="text-[#333] lg:text-xs text-[0.5385rem] font-ralewayBold leading-[150%]">DEVELOPMENT</span>
                        <span class="text-[#999] lg:text-xs text-[0.5385rem] font-ralewayMedium leading-[150%]">11 March 2023</span>
                    </div>
                    <h4 class="text-[#333] lg:text-[2rem] md:text-[1.43606rem] text-[1.07rem] lg:mb-[0.44rem] mb-[1.69rem] font-ralewayBold lg:leading-[2.8125rem] leading-[1.51944rem] md:tracking-[-0.0625rem]">How to build strong portfolio and get a Job in UI/UX</h4>
                    <h5 class="text-[#666] lg:text-base text-[0.718rem] lg:mb-[2.38rem] mb-[1.31rem] leading-[150%]">Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from</h5>
                    <button class="text-[#7C4EE4] lg:text-lg text-[0.80775rem] font-ralewayBold leading-[150%] underline">Read More...</button>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="bg-[#7C4EE4] lg:h-[33.375rem] h-[24.25rem] flex justify-center items-center">
        <div class="container mx-auto lg:px-0 px-6 text-center flex flex-col justify-center items-center">
            <h2 class="lg:mb-12 mb-[2.19rem] text-white text-center lg:text-[3.25rem] md:text-[2.33rem] text-[1.5rem] max-w-3xl font-ralewayBold lg:leading-[3rem] leading-[2.15406rem] tracking-[0.0125rem]">Get our stories delivered From us to your inbox weekly.</h2>
            <div class="flex items-center justify-center gap-2 w-full mb-6">
                <input type="text" class="bg-white rounded-lg outline-none lg:text-base text-[0.66194rem] lg:h-14 h-[2.31rem] lg:px-[1.44rem] px-[0.95rem] w-full max-w-[20rem] text-[#5A7184] placeholder:opacity-75 leading-[normal]" placeholder="Your Email">
                <button class="rounded-lg border-2 border-solid border-white lg:h-14 h-[2.31rem] lg:px-8 px-[1.4rem] text-white mg:text-lg text-[0.74469rem] font-ralewayBold leading-[normal] min-w-fit">Get started</button>
            </div>
            <p class="text-[#BBB] text-center lg:text-base text-[0.718rem] max-w-[34.6875rem] leading-7">Get a response tomorrow if you submit by 9pm today. If we received after 9pm will get a reponse the following day.</p>
        </div>
    </section>

    <footer class="md:py-[3.19rem] py-[2.29rem]">
        <div class="container mx-auto flex flex-col items-center">
            <div class="flex items-center lg:gap-[0.94rem] gap-[0.68rem] lg:mb-[2.63rem] mb-[1.8rem]">
                <svg class="lg:w-[44px] lg:h-[44px] w-[32px] h-[32px]" width="44" height="44" viewBox="0 0 44 44" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M4.88945 38.9723C1.09221 35.2276 -0.689229 29.5324 0.381427 24.2982C1.44056 18.4198 6.00621 13.2958 11.7719 11.6808C14.5945 14.5445 17.453 17.3696 20.2885 20.2179C20.8725 20.7814 21.4078 21.3949 22.0379 21.9084C20.0285 21.9289 18.0152 21.8546 16.0084 21.9327C13.2357 22.1082 10.8869 24.7234 11.0419 27.5037C11.0163 30.3097 13.5328 32.8455 16.3401 32.8288C21.8624 32.8417 27.3835 32.8276 32.9033 32.8378C36.5314 36.4698 40.1532 40.1096 43.8006 43.7237C43.2371 43.8312 42.6647 43.8018 42.096 43.7967C33.5807 43.798 25.068 43.7967 16.5553 43.798C12.238 43.8095 7.92469 42.0575 4.88945 38.9723Z" fill="#7C4EE4"/><path d="M10.7578 10.713C7.16802 7.14752 3.63331 3.52317 -1.40422e-06 -3.8147e-06C8.49865 0.0332943 16.996 0.00511477 25.4947 0.0153607C26.9214 0.0345714 28.3621 -0.0653203 29.7722 0.202346C33.3863 0.700533 36.8096 2.46916 39.3108 5.12275C42.0911 8.00558 43.7176 11.9475 43.8444 15.9459C43.9392 19.2411 43.0068 22.5619 41.2228 25.3333C39.1238 28.5568 35.8798 31.1054 32.1479 32.1248C29.3611 29.2932 26.5308 26.5013 23.726 23.6851C23.1613 23.1613 22.6874 22.5337 22.0394 22.1008C22.1495 22.0099 22.2686 21.9331 22.3993 21.8716C24.1807 21.9087 25.966 21.9036 27.7487 21.8806C30.515 21.8037 32.9432 19.2756 32.8881 16.5055C32.9688 14.2553 31.446 12.0935 29.347 11.3213C28.5466 10.9755 27.6629 10.9704 26.8061 10.9781C21.6347 10.9832 16.4645 10.9768 11.2944 10.9819C11.078 10.9832 10.8987 10.8935 10.7578 10.713Z" fill="#7C4EE4"/></svg>
                <span class="text-[#333] lg:text-[2.106rem] font-ralewayExtraBold leading-[normal] text-[1.51213rem]">Zarrin</span>
            </div>
            <div class="flex items-center lg:gap-14 gap-8">
                <button class="text-[#150E06] lg:text-base text-[0.718rem] leading-[150%]">Home</button>
                <button class="text-[#150E06] lg:text-base text-[0.718rem] leading-[150%]">Blog</button>
                <button class="text-[#150E06] lg:text-base text-[0.718rem] leading-[150%]">About</button>
                <button class="text-[#150E06] lg:text-base text-[0.718rem] leading-[150%]">Contact Us</button>
            </div>
            <div class="flex items-center gap-4 lg:my-10 my-[1.81rem]">
                <button class="bg-[#7C4EE4] lg:w-10 w-[1.8rem] lg:h-10 h-[1.8rem] lg:text-base text-[0.718rem] rounded-full grid place-content-center text-white font-ralewayBold leading-[150%]">FB</button>
                <button class="bg-[#7C4EE4] lg:w-10 w-[1.8rem] lg:h-10 h-[1.8rem] lg:text-base text-[0.718rem] rounded-full grid place-content-center text-white font-ralewayBold leading-[150%]">IG</button>
                <button class="bg-[#7C4EE4] lg:w-10 w-[1.8rem] lg:h-10 h-[1.8rem] lg:text-base text-[0.718rem] rounded-full grid place-content-center text-white font-ralewayBold leading-[150%]">LN</button>
                <button class="bg-[#7C4EE4] lg:w-10 w-[1.8rem] lg:h-10 h-[1.8rem] lg:text-base text-[0.718rem] rounded-full grid place-content-center text-white font-ralewayBold leading-[150%]">YT</button>
            </div>
            <hr class="border-[#7C4EE4] w-full mb-10">
            <span class="text-[#150E06] leading-[150%] lg:text-base text-[0.718rem]">Copyright Lazri Ossama © 2023. All Right Reserved</span>
        </div>
    </footer>

</div>