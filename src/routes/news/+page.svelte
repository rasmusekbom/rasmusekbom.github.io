<script>
    import Typewriter from 'svelte-typewriter'
    import { base } from '$app/paths'; 
  </script>
  
  <style>
    .app-container {
      background-image: url('https://static.vecteezy.com/system/resources/previews/027/203/947/non_2x/winter-landscape-illustration-winter-background-with-frozen-lake-and-dead-tree-silhouette-of-cold-season-landscape-for-background-wallpaper-display-or-landing-page-snow-landscape-with-pine-vector.jpg');
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }
  </style>
  
  <div class="app-container">
    <div class="text-center w-full mt-12">
      <Typewriter>
      <h1 class="text-5xl font-bold text-orange-500 bg-orange-100 bg-opacity-60 p-2">
        CS2 NEWS AND INFORMATION
      </h1>
    </Typewriter>
    <Typewriter>
      <h3 class="text-3xl font-semibold text-orange-400 mt-5 bg-orange-50 bg-opacity-80 p-2">
        READ AND BECOME ENLIGHTENED
      </h3>
    </Typewriter>
    </div>
  
    <div class="text-center mt-8 opacity-80">
        <a href="{base}/" class="mt-4 mr-4 rounded-full bg-white px-4 py-2.5 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-200">REF CODES</a>
        <a href="{base}/news" class="mt-4 mr-4 rounded-full bg-white px-4 py-2.5 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-200">CS2 NEWS</a>
        <a href="{base}/giveaways" class="mt-4 mr-4 rounded-full bg-white px-4 py-2.5 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-200">GIVEAWAYS</a>
        <a href="{base}/videos" class="mt-4 mr-4 rounded-full bg-white px-4 py-2.5 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-200">CS2 VIDEOS</a>
        <a href="{base}/blog" class="mt-4 rounded-full bg-white px-4 py-2.5 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-200">BLOG POSTS</a>
      </div>
  
          <div class="opacity-85 grid lg:grid-cols-4 md:grid-cols-2 sm:grid-cols-1 gap-6 ml-5 mt-8 mr-5">
            <article class="relative isolate flex flex-col justify-end overflow-hidden rounded-2xl bg-gray-900 px-8 pb-8 pt-80 sm:pt-48 lg:pt-80">
              <img src="https://img-cdn.hltv.org/gallerypicture/24WDnQWeF7Im31MI8hk-aK.png?auto=compress&fm=avif&ixlib=java-2.1.0&q=75&w=800&s=773267c4ef12bb73f9a59dd7ac097e3f" alt="" class="absolute inset-0 -z-10 h-full w-full object-cover">
              <div class="absolute inset-0 -z-10 bg-gradient-to-t from-gray-900 via-gray-900/40"></div>
              <div class="absolute inset-0 -z-10 rounded-2xl ring-1 ring-inset ring-gray-900/10"></div>
      
              <div class="flex flex-wrap items-center gap-y-1 overflow-hidden text-sm leading-6 text-gray-300">
                <time datetime="2020-03-16" class="mr-8">Dec 27, 2023 - Ongoing</time>
                <div class="-ml-4 flex items-center gap-x-4">
                  <svg viewBox="0 0 2 2" class="-ml-0.5 h-0.5 w-0.5 flex-none fill-white/50">
                    <circle cx="1" cy="1" r="1" />
                  </svg>
                  <div class="flex gap-x-2.5">
                    <img src="https://pbs.twimg.com/profile_images/1472654373331390464/mDvubk1O_400x400.jpg" alt="" class="h-6 w-6 flex-none rounded-full bg-white/10">
                    LucasAM, HLTV
                  </div>
                </div>
              </div>
              <h3 class="mt-3 text-lg font-semibold leading-6 text-white">
                <a href="https://www.hltv.org/news/37845/top-20-players-of-2023-introduction" target="_blank">
                  <span class="absolute inset-0"></span>
                  TOP 20 PLAYERS OF 2023
                </a>
              </h3>
            </article>

            <article class="relative isolate flex flex-col justify-end overflow-hidden rounded-2xl bg-gray-900 px-8 pb-8 pt-80 sm:pt-48 lg:pt-80">
                <img src="https://www.dexerto.com/cdn-cgi/image/width=3840,quality=75,format=auto/https://editors.dexerto.com/wp-content/uploads/2023/09/01/cs2-best-settings.jpg" alt="" class="absolute inset-0 -z-10 h-full w-full object-cover">
                <div class="absolute inset-0 -z-10 bg-gradient-to-t from-gray-900 via-gray-900/40"></div>
                <div class="absolute inset-0 -z-10 rounded-2xl ring-1 ring-inset ring-gray-900/10"></div>
        
                <div class="flex flex-wrap items-center gap-y-1 overflow-hidden text-sm leading-6 text-gray-300">
                  <time datetime="2020-03-16" class="mr-8">Ongoing</time>
                  <div class="-ml-4 flex items-center gap-x-4">
                    <svg viewBox="0 0 2 2" class="-ml-0.5 h-0.5 w-0.5 flex-none fill-white/50">
                      <circle cx="1" cy="1" r="1" />
                    </svg>
                    <div class="flex gap-x-2.5">
                      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Steam_icon_logo.svg/2048px-Steam_icon_logo.svg.png" alt="" class="h-6 w-6 flex-none rounded-full bg-white/10">
                      Steam
                    </div>
                  </div>
                </div>
                <h3 class="mt-3 text-lg font-semibold leading-6 text-white">
                  <a href="https://www.counter-strike.net/news/updates" target="_blank">
                    <span class="absolute inset-0"></span>
                    CS2 OFFICIAL CHANGELOG
                  </a>
                </h3>
              </article>

              <article class="relative isolate flex flex-col justify-end overflow-hidden rounded-2xl bg-gray-900 px-8 pb-8 pt-80 sm:pt-48 lg:pt-80">
                <img src="https://ih1.redbubble.net/image.5278921732.2930/flat,750x,075,f-pad,750x1000,f8f8f8.jpg" alt="" class="absolute inset-0 -z-10 h-full w-full object-cover">
                <div class="absolute inset-0 -z-10 bg-gradient-to-t from-gray-900 via-gray-900/40"></div>
                <div class="absolute inset-0 -z-10 rounded-2xl ring-1 ring-inset ring-gray-900/10"></div>
        
                <div class="flex flex-wrap items-center gap-y-1 overflow-hidden text-sm leading-6 text-gray-300">
                  <time datetime="2020-03-16" class="mr-8">Ongoing</time>
                  <div class="-ml-4 flex items-center gap-x-4">
                    <svg viewBox="0 0 2 2" class="-ml-0.5 h-0.5 w-0.5 flex-none fill-white/50">
                      <circle cx="1" cy="1" r="1" />
                    </svg>
                    <div class="flex gap-x-2.5">
                      <img src="https://pbs.twimg.com/profile_images/1679836827623014402/zNJmLHuu_400x400.jpg" alt="" class="h-6 w-6 flex-none rounded-full bg-white/10">
                      CS2 Staff
                    </div>
                  </div>
                </div>
                <h3 class="mt-3 text-lg font-semibold leading-6 text-white">
                  <a href="https://twitter.com/cs2newsupdate" target="_blank">
                    <span class="absolute inset-0"></span>
                    CS2 OFFICIAL NEWS TWITTER
                  </a>
                </h3>
              </article>

              
              <article class="relative isolate flex flex-col justify-end overflow-hidden rounded-2xl bg-gray-900 px-8 pb-8 pt-80 sm:pt-48 lg:pt-80">
                <img src="https://www.esports.net/wp-content/uploads/2019/07/logo-esports-net-dark.jpg" alt="" class="absolute inset-0 -z-10 h-full w-full object-cover">
                <div class="absolute inset-0 -z-10 bg-gradient-to-t from-gray-900 via-gray-900/40"></div>
                <div class="absolute inset-0 -z-10 rounded-2xl ring-1 ring-inset ring-gray-900/10"></div>
        
                <div class="flex flex-wrap items-center gap-y-1 overflow-hidden text-sm leading-6 text-gray-300">
                  <time datetime="2020-03-16" class="mr-8">Mar 16, 2020</time>
                  <div class="-ml-4 flex items-center gap-x-4">
                    <svg viewBox="0 0 2 2" class="-ml-0.5 h-0.5 w-0.5 flex-none fill-white/50">
                      <circle cx="1" cy="1" r="1" />
                    </svg>
                    <div class="flex gap-x-2.5">
                      <img src="https://pbs.twimg.com/profile_images/1149341314410065920/jusTPTA2_400x400.png" alt="" class="h-6 w-6 flex-none rounded-full bg-white/10">
                      ESPORTS.NET
                    </div>
                  </div>
                </div>
                <h3 class="mt-3 text-lg font-semibold leading-6 text-white">
                  <a href="https://www.esports.net/news/counter-strike/" target="_blank">
                    <span class="absolute inset-0"></span>
                    E-SPORTS CS2 NEWS
                  </a>
                </h3>
              </article>

      
            <!-- More posts... -->
          </div>
      </div>
      
    
  