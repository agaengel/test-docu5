<template>
  <!-- card view -->
  <div class="bg-white h-full overflow-hidden rounded-lg shadow-lg flex-1">
    <!-- card header -->
    <g-link class="block relative overflow-hidden" :to="item.node.path">
      <picture class="flex-1">
        <g-image :alt="item.node.image_caption" :src="item.node.image" />
      </picture>
    </g-link>
    <!-- card content -->
    <div class="p-8">
      <h2>
        <g-link class="block hover:text-pink-500" :to="item.node.path">{{
          item.node.title
        }}</g-link>
      </h2>
      <div class="flex flex-col text-base md:flex mb-4">
        <div>{{ item.node.author.name }}</div>
        <div class="hidden md:block px-2"></div>
        <time :datetime="item.node.datetime">{{ item.node.humanTime }}</time>
      </div>
      <ul class="flex flex-wrap border-t border-gray-100">
        <li class="mr-2 mt-2" v-for="tag in item.node.tags" :key="tag.id">
          <g-link
            :to="tag.path"
            class="inline-block border border-pink-300 px-4 py-2 text-pink-500 text-xs font-semibold rounded hover:text-white hover:bg-pink-500 hover:border-pink-500"
          >{{ tag.title }}
          </g-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SampleCard',
  props: {
    item: {
      type: Object,
      default: function () {
        return {}
      },
    },
  },
}
</script>
