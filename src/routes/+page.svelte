<script lang="ts">
    import { onMount } from 'svelte';

    let mapSquare = $state("./avatar_normal.png");

</script>

<svelte:head>
  <title>hieri.net</title>
  <meta name="description" content="website" />
</svelte:head>

<main class="container mx-auto dark:bg-gray-900 dark:text-white min-h-screen">
  <h1 class="text-center text-6xl mt-3 mb-10">hieri.net</h1>

  <div class="text-center mb-10">
    <img
      alt="avatar"
      src={mapSquare}
      onmouseenter={() => { mapSquare = "./avatar_smile.png"; }}
      onmouseleave={() => { mapSquare = "./avatar_normal.png"; }}
      class="inline hover:cursor-grab w-1/2" 
    />
  </div>

  <div class="text-4xl mt-20 mb-10">
    <h1 class="text-left mb-5">
      <a href="https://www.lovelive-anime.jp/otonokizaka/member/member02.html" target="_blank" rel="noopener noreferrer" class="underline decoration-blue-300">絢瀬絵里</a>
      を推しましょう絶対に。
    </h1>
    <h1 class="text-left mb-5">
    <a href="https://nbcuni-music.com/yoshino_nanjo/" target="_blank" rel="noopener noreferrer" class="underline decoration-blue-300">南條愛乃さん</a>
    も推しましょう絶対に。</h1>
    <h1 class="text-left mb-5">
      南條さんの
      <a href="https://www.dlsite.com/home/fsr/=/keyword/ASMR/keyword_creater/%22%E5%8D%97%E6%A2%9D%E6%84%9B%E4%B9%83%22/age_category[0]/general/order/trend/options[0]/JPN/options[1]/NM" target="_blank" rel="noopener noreferrer" class="underline decoration-blue-300">ASMR作品</a>
      をぜひ聴いて下さい絶対に。
    </h1>
  </div>

  <div>
    <h1 class="text-3xl mt-3 mb-3 text-center">
      <a href="/profile" class="underline decoration-blue-300">プロフィール</a>
    </h1>
    <h1 class="text-3xl mt-3 mb-3 text-center">
      <a href="/game" class="underline decoration-blue-300">ゲーム</a>
    </h1>
  </div>

  <div class="grid grid-cols-1 lg:grid-cols-2 items-end mb-5">
    <div class="grid justify-items-center lg:justify-items-start">
      <img
        src="https://spotify-recently-played-readme.vercel.app/api?user=31upypeuqy2n3urisvkknr7gh2ra"
        alt="recently spotify"
        loading="lazy"
        class="right-0"
      />
    </div>
    <div class="grid justify-items-center lg:justify-items-end">
      <img
        src="https://moe-counter-cf.yude.workers.dev/hieri"
        alt="表示カウンター"
        loading="lazy"
        class="w-1/2"
      />
    </div>
  </div>

  <hr />
  <div class="text-center mb-2 mt-1">
    <img alt="hieribanner" src="./website_banner.png" class="h-12 inline" />
    <img alt="happybanner" src="./busy_banner.webp" class="h-12 inline" />
  </div>
  <p class="text-center text-xl">
    <a href="https://Github.com/hieri1021/hieri.net" target="_blank" rel="noopener noreferrer" class="underline decoration-blue-300">Github</a>
    /
    <a href="https://twitter.com/yamahi_5028" target="_blank" rel="noopener noreferrer" class="underline decoration-blue-300">Twitter</a>
    /
    <a href="https://scrapbox.io/hieri-scrapbox" target="_blank" rel="noopener noreferrer" class="underline decoration-blue-300">Scrapbox</a>
  </p>
</main>