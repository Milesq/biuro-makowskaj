<template>
  <v-main>
    <div v-for="post in posts" :key="post.title">
      <BlogPost
        :title="post.title"
        :image="post.image"
        :description="post.description"
        :date="post.date"
      />
    </div>
  </v-main>
</template>

<script lang="ts">
import Vue from 'vue';
import BlogPost from '../../components/BlogPost.vue';

export default Vue.extend({
  components: {
    BlogPost,
  },
  data() {
    return {
      posts: [
        {
          title: 'Lorem Ipsum',
          image: '',
          description:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Nunc non blandit massa enim. Non sodales neque sodales ut etiam sit. Proin fermentum leo vel orci. Vel orci porta non pulvinar neque laoreet suspendisse. Elementum integer enim neque volutpat ac. Ornare lectus sit amet est placerat in egestas. Est ullamcorper eget nulla facilisi etiam dignissim diam. Id faucibus nisl tincidunt eget. Sit amet consectetur adipiscing elit ut. Non blandit massa enim nec dui nunc. Ultrices eros in cursus turpis massa tincidunt dui ut ornare.',
          date: new Date('Dec 10, 2020 01:00:00'),
        },
        {
          title: 'Lorem Ipsum',
          image:
            'https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwallpapertag.com%2Fwallpaper%2Ffull%2Fb%2Fe%2F7%2F298063-download-free-grass-background-1920x1200.jpg&f=1&nofb=1',
          description:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Nunc non blandit massa enim. Non sodales neque sodales ut etiam sit. Proin fermentum leo vel orci. Vel orci porta non pulvinar neque laoreet suspendisse. Elementum integer enim neque volutpat ac. Ornare lectus sit amet est placerat in egestas. Est ullamcorper eget nulla facilisi etiam dignissim diam. Id faucibus nisl tincidunt eget. Sit amet consectetur adipiscing elit ut. Non blandit massa enim nec dui nunc. Ultrices eros in cursus turpis massa tincidunt dui ut ornare.',
          date: new Date(),
        },
        {
          title: 'Lorem Ipsum',
          image: '',
          description:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Nunc non blandit massa enim. Non sodales neque sodales ut etiam sit. Proin fermentum leo vel orci. Vel orci porta non pulvinar neque laoreet suspendisse. Elementum integer enim neque volutpat ac. Ornare lectus sit amet est placerat in egestas. Est ullamcorper eget nulla facilisi etiam dignissim diam. Id faucibus nisl tincidunt eget. Sit amet consectetur adipiscing elit ut. Non blandit massa enim nec dui nunc. Ultrices eros in cursus turpis massa tincidunt dui ut ornare. Lacus laoreet non curabitur gravida arcu ac tortor. Est ante in nibh mauris cursus. Vulputate eu scelerisque felis imperdiet proin. Lectus sit amet est placerat in egestas. Lectus arcu bibendum at varius. Aliquam nulla facilisi cras fermentum odio. Pharetra et ultrices neque ornare aenean euismod elementum nisi quis. Felis eget velit aliquet sagittis id consectetur purus ut. Praesent semper feugiat nibh sed pulvinar proin. Vitae proin sagittis nisl rhoncus mattis rhoncus urna. Consequat interdum varius sit amet mattis vulputate enim nulla. Vitae auctor eu augue ut. Egestas erat imperdiet sed euismod nisi porta lorem.',
          date: new Date(),
        },
      ],
    };
  },
});
</script>
