<template>
  <div class="grid grid-cols-1 md:grid-cols-2 gap-8 p-4 md:mx-20">
    <div
      class="w-full rounded overflow-hidden box-shadow flex justify-center items-center pic-container">
      <img class="w-full" :src="url" alt="Image Description">
    </div>

    <div>
      <div class="font-bold text-xl mb-2">
        Painting Name
      </div>
      <div class="flex items-center mb-4">
        <img class="w-10 h-10 rounded-full mr-4" src="/unsplash_iEEBWgY_6lA.png" alt="Avatar of artist">
        <div class="text-sm">
          <p class="leading-none blue-text">
            artist
          </p>
        </div>
      </div>
      <div class="mb-2">
        <div class="flex items-center">
          <div class="vl pr-2">
            <p class="text-sm flex items-center text-black">
              watercolor on canvas
            </p>
          </div>
          <div class="pl-2">
            <p class="text-sm flex items-center text-black">
              24” x 12”
            </p>
          </div>
        </div>
      </div>
      <div class="mb-8">
        <div class="flex items-center">
          <div class="pr-2 vl">
            <span class="rounded p-2 price-box">$46</span>
          </div>
          <div class="px-2 vl">
            <p class="text-sm flex items-center blue-text">
              <FavoriteOutline />&nbsp;favorite
            </p>
          </div>
          <div class="pl-2 pr-4">
            <p class="text-sm flex items-center blue-text">
              <ShareOutline />&nbsp;share
            </p>
          </div>
          <div class="pl-2">
            <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
              order
            </button>
          </div>
        </div>
      </div>
      <div class="mb-8">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit.
          Aliquet volutpat faucibus tellus tristique dui.
          Suscipit cursus eget imperdiet ullamcorper non adipiscing.
          Sapien diam turpis nulla feugiat sit.
        </p>
      </div>
      <div class="mb-4">
        <hr>
      </div>
      <div>
        <div class="font-bold text-md mb-2">
          Additional Details
        </div>
        <ul class="list-inside">
          <li>Added 12/2/21</li>
          <li>Located in St. Petersburg</li>
          <li>14 day cancellation period</li>
          <li>Delivery usually 14 days</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import FavoriteOutline from './icons/FavoriteOutline'
import ShareOutline from './icons/ShareOutline'

export default {
  name: 'PicPreview',
  components: { FavoriteOutline, ShareOutline },

  props: {
    url: { type: String }
  }
}
</script>
<style lang="css">
  .vl {
    border-right: 1px solid #E6E6E6;
  }

  .blue-text {
    color: #1039A2;
  }

  .price-box {
    background-color: #CCF3CB;
    color: #038800;
  }

  .pic-container {
    justify-self: center;
    height: 30rem;
  }

  @media screen(sm) {
    .pic-container {
      height: initial;
    }
  }
  .list-inside {
    list-style: inside;
  }
  .box-shadow{
    border: 1px solid #F2F2F2;
    box-sizing: border-box;
    box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
  }
</style>
