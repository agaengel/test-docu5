<template>
  <Layout>
    <section class="container mx-auto">
      <h1>
        All
        <g-link to="/samples">samples</g-link>
        tagged as
        <a
          v-if="$page.sampleTag.url"
          :href="$page.sampleTag.url"
          target="_blank"
          rel="noopener"
        >
          "{{ $page.sampleTag.title }}"
        </a>
        <span v-else> "{{ $page.sampleTag.title }}" </span>
      </h1>
      <p
        v-if="$page.sampleTag.description"
        v-html="$page.sampleTag.description"
      ></p>

      <div class="flex flex-wrap -mx-2">
        <div
          class="w-full max-w-sm lg:w-1/3 mb-8 px-2"
          v-for="element in $page.sampleTag.belongsTo.edges"
          :key="element.node.id"
        >
          <SampleCard :item="element" />
        </div>
      </div>
    </section>
  </Layout>
</template>

<page-query>
query($id: ID!) {
  sampleTag(id: $id) {
    title
    url
    description
    belongsTo {
      edges {
        node {
          ... on Sample {
            id
            title
            path
            excerpt
            image(height: 300, width: 423, fit: cover)
            humanTime: created(format: "Do MMMM YYYY")
            datetime: created(format: "ddd MMM DD YYYY hh:mm:ss zZ")
            author {
              name
            }
            tags {
              id
              title
              path
            }
          }
        }
      }
    }
  }
}
</page-query>

<script>
import SampleCard from '@/components/SampleCard'

export default {
  metaInfo: {
    title: 'SampleTags',
  },
  components: {
    SampleCard,
  },
}
</script>
