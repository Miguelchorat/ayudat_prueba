<template>
  <main class="home">
    <JoinSection />
    <PopularSection />
    <CourseSection />
    <PackageSection />
    <ReviewSection />
    <FaqSection />
    <NewsletterSection />
  </main>
</template>
<script>

import JoinSection from '@/components/JoinSection.vue';
import PopularSection from '@/components/PopularSection.vue';
import CourseSection from '@/components/CourseSection.vue';
import PackageSection from '@/components/PackageSection.vue';
import ReviewSection from '@/components/ReviewSection.vue';
import FaqSection from '@/components/FaqSection.vue';
import NewsletterSection from '@/components/NewsletterSection.vue';

export default {
  components: {
    JoinSection,
    PopularSection,
    CourseSection,
    PackageSection,
    ReviewSection,
    FaqSection,
    NewsletterSection
  }
}
</script>
