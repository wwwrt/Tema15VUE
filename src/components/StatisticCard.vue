<script setup>
defineProps({
  details:{
    type: Object,
    required: true
  }
})
</script>

<template>
  <div
    class="relative flex w-full max-w-[26rem] p-4 border shadow-md flex-col rounded-xl bg-transparent bg-clip-border text-gray-700">
    <div
      class="relative flex items-center gap-4 pt-0 pb-2 mx-0 mt-4 overflow-hidden text-gray-700 bg-transparent shadow-none rounded-xl bg-clip-border">
      <img
        :src="details.icon"
        class="relative inline-block h-[58px] w-[58px] !rounded-full  object-cover object-center" />
      <div class="flex w-full flex-col gap-0.5">
        <div class="flex items-center justify-between">
          <h5 class="block font-sans text-xl antialiased font-semibold leading-snug tracking-normal text-blue-gray-900">
            {{ details.name}}
          </h5>
          <div class="flex items-center gap-0 5">
            <i class="bi bi-bookmark-fill"></i>
          </div>
        </div>
      </div>
    </div>

    <h2 class="block font-sans text-4xl antialiased font-semibold leading-snug tracking-normal text-blue-gray-900">
      {{details.new}} {{ details.unit }}
    </h2>
    <div class="p-0 mb-6">

      <p class="block font-sans text-base antialiased font-light leading-relaxed text-inherit">
       {{details.last}} {{ details.what }}

      </p>
      <p class="block font-sans text-base antialiased font-light leading-relaxed text-inherit">
        {{ details.info }}

      </p>
    </div>
  </div>

</template>