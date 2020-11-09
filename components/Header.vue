<template>
  <header class="max-w-5xl mx-auto py-8 flex">
    <nav>
      <ul>
        <li>
          <nuxt-link
            class="text-teal-600 hover:underline"
            to="/">
            Home
          </nuxt-link>
        </li>
        <li>
          <nuxt-link
            class="text-teal-600 hover:underline"
            to="/articles">
            Blog
          </nuxt-link>
        </li>
      </ul>
    </nav>
    <div class="flex-1">
      <a href="/" class="block w-56 mx-auto">
        <img src="https://mma.prnewswire.com/media/555056/ASTOUND_Group_Inc__ASTOUND_Building_the_Future_with_EDIT.jpg?p=facebook">
      </a>
    </div>
    <nav>
      <ul>
        <li>
          <nuxt-link
            class="text-teal-600 hover:underline"
            to="/en/blog">
            English
          </nuxt-link>
        </li>
        <li>
          <nuxt-link
            class="text-teal-600 hover:underline"
            to="/de/blog">
            German
          </nuxt-link>
        </li>
      </ul>
    </nav>
  </header>
</template>