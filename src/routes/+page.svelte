<script>
  import { onMount } from 'svelte';
  import Typewriter from 'svelte-typewriter'
  import { quintOut } from 'svelte/easing';
  import { scale } from 'svelte/transition';
  import { base } from '$app/paths';

  let animate = false;

  onMount(() => {
    setTimeout(() => {
      animate = true;
    }, 100);
  });

  let people = [
    {
      name: 'CSGOEMPIRE.com',
      title: 'Code: KungKhalifa',
      role: '3 FREE CHANCES ON A DRAGON LORE',
      url: 'https://csgoempire.com/r/kungkhalifa',
      imageUrl: 'https://csgoempire.com/assets/coin-bonus-u3uE7Jsu.png'
    },
    {
      name: 'CSGOROLL.com',
      title: 'Code: FREECASE20',
      role: '5% DEPOSIT BONUS & 3 FREE CASES',
      url: 'https://csgoroll.com/r/FREECASE20',
      imageUrl: 'https://s3-eu-west-1.amazonaws.com/tpd/logos/59a445bb0000ff0005a9deb9/0x0.png'
    },
    {
      name: 'HELLCASE.com',
      title: 'Code: KungKhalifa',
      role: '+10% DEPOSIT BONUS',
      url: 'https://hellcase.com/fkungkhalifa',
      imageUrl: 'https://media.licdn.com/dms/image/C560BAQFleZOlS4WLkQ/company-logo_200_200/0/1631330559671?e=2147483647&v=beta&t=3f8r5C8vxPG0TA58U-aRJr2hqp_CAG6JmXkVS52Zx5w'
    },
    {
      name: 'GAMDOM.com',
      title: 'Code: KungKhalifa',
      role: '+10% DEPOSIT BONUS',
      url: 'https://gamdom.com/r/kungkhalifa',
      imageUrl: 'https://s3-eu-west-1.amazonaws.com/tpd/logos/598f37240000ff0005a8b68f/0x0.png'
    },
  ];

  const columnsPerRow = 5;
  const rows = Math.ceil(people.length / columnsPerRow);

  let rowsArray = Array.from({ length: rows }, (_, index) =>
    people.slice(index * columnsPerRow, (index + 1) * columnsPerRow)
  );
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
      GRAB FREE CASES AND RECEIVE MORE BALANCE WHEN DEPOSITING!
    </h1>
  </Typewriter>
  <Typewriter>
    <h3 class="text-3xl font-semibold text-orange-400 mt-5 bg-orange-50 bg-opacity-80 p-2">
      USE THE REFERRAL CODES BELOW
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

  <div class="grid lg:grid-cols-4 md:grid-cols-2 sm:grid-cols-1 gap-6 ml-5 mt-8 mr-5">
    {#each rowsArray as row (row)}
    {#if animate}
      {#each row as person (person.name)}
        <div transition:scale={{ duration: 300, easing: quintOut, x: animate ? 1 : 0 }}>
          <div class="col-span-1 flex flex-col divide-y divide-gray-200 rounded-lg bg-gray-100 bg-opacity-95 text-center shadow-blue-300 shadow-xl" key={person.name}>
            <div class="flex flex-1 flex-col p-8">
              <img class="mx-auto h-32 w-32 flex-shrink-0 rounded-full" src={person.imageUrl} alt={person.name}>
              <h3 class="mt-6 text-2xl font-medium text-gray-900">{person.name}</h3>
              <dl class="mt-1 flex flex-grow flex-col justify-between">
                <dt class="sr-only">Title</dt>
                <dd class="text-lg text-gray-700 font-bold">{person.title}</dd>
                <dt class="sr-only">Role</dt>
                <dd class="mt-3">
                  <span class="inline-flex items-center rounded-full bg-green-50 px-2 py-1 text-md font-medium text-green-700 ring-1 ring-inset ring-green-600/20">{person.role}</span>
                </dd>
              </dl>
            </div>
            <div>
              <div class="-mt-px flex divide-x divide-yellow-900">
                <div class="-ml-px flex w-0 flex-1">
                  <a href={person.url} target="_blank" class="relative inline-flex w-0 flex-1 items-center justify-center gap-x-3 rounded-br-lg border border-green-200 py-4 text-xl font-semibold text-gray-900">
                    <svg class="h-6 w-6 flex-none text-gray-500" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
                      <path stroke-linecap="round" stroke-linejoin="round" d="M9.568 3H5.25A2.25 2.25 0 003 5.25v4.318c0 .597.237 1.17.659 1.591l9.581 9.581c.699.699 1.78.872 2.607.33a18.095 18.095 0 005.223-5.223c.542-.827.369-1.908-.33-2.607L11.16 3.66A2.25 2.25 0 009.568 3z" />
                      <path stroke-linecap="round" stroke-linejoin="round" d="M6 6h.008v.008H6V6z" />
                    </svg>
                    VISIT PAGE WITH REF CODE
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
        
      {/each}
      {/if}
    {/each}
  </div>
  <h3 class="text-center text-3xl font-semibold text-orange-400 mt-20 bg-orange-50 bg-opacity-80 p-2">
    CHECK WEEKLY FOR NEW CODES AND SITES!
  </h3>
  <h3 class="text-center text-xl font-semibold text-white-400 mt-4 bg-orange-50 bg-opacity-80 p-2">
    <a href="https://twitter.com/KungKhalifa" target="_blank">Do you want to promote your code here to be viewed by thousands of visitors weekly? Reach out to us at Twitter @KungKhalifa for more information</a>
    
  </h3>
</div>
