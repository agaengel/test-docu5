<template>
  <Layout>
    <section class="container mx-auto">
      <div class="subheader">
        <h1>Blog</h1>
        <p>Get inspired</p>
      </div>
      <div class="content">
        <div class="flex flex-wrap -mx-2">
          <div
            class="w-full flex-none max-w-sm lg:w-1/3 mb-8 px-2"
            v-for="entry in $page.allBlog.edges"
            :key="entry.node.id"
          >
            <SampleCard :item="entry" />
          </div>
        </div>
      </div>
    </section>
  </Layout>
</template>

<script>
import SampleCard from '@/components/SampleCard'

export default {
  metaInfo: {
    title: 'Blog',
  },
  components: {
    SampleCard,
  },
}
</script>

<page-query>
query {
  allBlog(sortBy: "created") {
    edges {
      node {
        id
        title
        excerpt
        samplepath: path(to: "sample")
        path
        image(height: 300, width: 423, fit: cover)
        humanTime: created(format: "Do MMMM YYYY")
        datetime: created(format: "ddd MMM DD YYYY hh:mm:ss zZ")
        author {
          name
        }
        category {
          title
        }
        tags {
          id
          title
          path
        }
        type
      }
    }
  }
}
</page-query>
