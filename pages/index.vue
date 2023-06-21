<script setup>
const items = [
  {
    id: 1,
    link: "https://p2p.onecause.com/2023-tcsnyc-marathon/team/eric-arbee-carolinas-section",
    title: "Donate to PGA Reach on my behalf",
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
    link: "https://willio.com",
    title: "Willio.com (my SaaS product)",
    class: "ring-sky-600",
  },
  {
    id: 4,
    link: "https://arbedigital.com",
    title: "My Digital Agency",
    class: "ring-red-500",
  },
];
</script>

<template>
  <div>
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
          I'm running in the NYC Marathon (in November) to raise money for PGA
          Reach. Please consider donating!
        </p>
      </div>
    </div>

    <ul role="list" class="space-y-3">
      <li
        v-for="item in items"
        :key="item.id"
        class="overflow-hidden bg-white px-4 py-4 sm:rounded-md sm:px-6 text-center"
      >
        <a
          href="{{ item.link }}"
          rel="noopener noreferrer"
          :class="`bg-white ${item.class} rounded bg-white px-4 py-2 text-sm font-semibold text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 hover:bg-gray-50`"
          >{{ item.title }}</a
        >
      </li>
    </ul>
  </div>
</template>
