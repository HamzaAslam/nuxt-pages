<template>
  <NuxtLayout>
    <div class="flex flex-col">
      <div class="prose">
        <h2>Dangggg</h2>
        <p>It looks like something broken</p>
        <p>
          <strong>{{ error.message }}</strong>
        </p>
      </div>
      <div>
        <p>
          Go to the
          <a href="" class="hover:cursor-pointer" @click="handleError"
            >First Lesson</a
          >
        </p>
      </div>
    </div>
  </NuxtLayout>
</template>

<script setup>
const error = useError();
const handleError = () => {
  clearError({
    redirect: `/course/chapter/1-chapter-1/lesson/1-introduction-to-typescript-with-vue-js-3`,
  });
};
</script>
