<script setup>
const items = [
  {
    id: 1,
    link: "https://give.pgareach.org/erickarbe",
    title: "Donate to PGA Reach on my behalf 🎉",
    class: "ring-indigo-600",
  },
  {
    id: 2,
    link: "https://erickar.be",
    title: "Read my Running Blog",
    class: "ring-green-600",
  },
  {
    id: 3,
    link: "https://sevenvictory.com",
    title: "Workout with me at Seven Victory",
    class: "ring-sky-600",
  },
  {
    id: 4,
    link: "https://arbedigital.com",
    title: "Arbé Digital",
    class: "ring-red-500",
  },
  {
    id: 5,
    link: "https://golfwebdesign.com",
    title: "Golf Web Design",
    class: "ring-green-500",
  },
];
</script>

<template>
  <div class="max-w-md mx-auto">
    <div class="flex p-6">
      <div class="mr-4 flex-shrink-0">
        <img
          class="inline-block h-14 w-14 rounded-full"
          src="/erick-avatar.jpeg"
          alt="Erick Arbe"
        />
      </div>
      <div>
        <h4 class="text-lg font-bold">Erick's Links</h4>
        <p class="mt-1">
          I'm running in the 2026 NYC Marathon (Nov. 1st) to raise money for PGA
          Reach. <strong>Please consider donating!</strong>
        </p>
      </div>
    </div>

    <ul role="list" class="space-y-3">
      <li
        v-for="item in items"
        :key="item.id"
        class="overflow-hidden px-4 py-4 sm:rounded-md sm:px-6 text-center"
      >
        <a
          :href="item.link"
          target="_blank"
          rel="noopener noreferrer"
          :class="`bg-white ${item.class} rounded bg-white px-4 py-2 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50`"
          >{{ item.title }}</a
        >
      </li>
    </ul>
  </div>
</template>
