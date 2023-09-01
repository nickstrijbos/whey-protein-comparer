<script>
  import WheyTable from "../components/WheyTable/WheyTable.svelte";
</script>

<nav
  class="bg-white dark:bg-gradient-to-r from-neutral-700 to-neutral-900 fixed w-full z-20 top-0 left-0 border-b border-neutral-200 dark:border-neutral-500"
>
  <div
    class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4"
  >
    <a href="/" class="flex items-center">
      <img
        src="../favicon.png"
        class="h-10 mr-3"
        alt="Whey Protein Comparer Logo"
      />
      <span
        class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"
        >Whey Protein Comparer</span
      >
    </a>
    <div class="flex md:order-2">
      <button
        type="button"
        class="text-white bg-neutral-700 hover:bg-neutral-800 focus:ring-4 focus:outline-none focus:ring-neutral-300 font-medium rounded-lg text-sm px-4 py-2 text-center mr-3 md:mr-0 dark:bg-neutral-600 dark:hover:bg-neutral-700 dark:focus:ring-neutral-800"
        >Get started</button
      >
      <button
        data-collapse-toggle="navbar-sticky"
        type="button"
        class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-neutral-500 rounded-lg md:hidden hover:bg-neutral-100 focus:outline-none focus:ring-2 focus:ring-neutral-200 dark:text-neutral-400 dark:hover:bg-neutral-700 dark:focus:ring-neutral-600"
        aria-controls="navbar-sticky"
        aria-expanded="false"
      >
        <span class="sr-only">Open main menu</span>
        <svg
          class="w-5 h-5"
          aria-hidden="true"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 17 14"
        >
          <path
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M1 1h15M1 7h15M1 13h15"
          />
        </svg>
      </button>
    </div>
    <div
      class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1"
      id="navbar-sticky"
    >
      <ul
        class="flex flex-col p-4 md:p-0 mt-4 font-medium border border-neutral-100 rounded-lg bg-neutral-500 md:flex-row md:space-x-8 md:mt-0 md:border-0 dark:bg-neutral-800 dark:border-neutral-700"
      >
        <li>
          <a
            href="/"
            class="block py-2 pl-3 pr-4 text-white bg-neutral-700 rounded md:bg-transparent md:text-neutral-700 md:p-0 md:dark:text-neutral-500"
            aria-current="page">Home</a
          >
        </li>
        <li>
          <a
            href="/"
            class="block py-2 pl-3 pr-4 text-neutral-900 rounded hover:bg-neutral-100 md:hover:bg-transparent md:hover:text-neutral-700 md:p-0 md:dark:hover:text-neutral-500 dark:text-white dark:hover:bg-neutral-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-neutral-700"
            >About</a
          >
        </li>

        <li>
          <a
            href="/"
            class="block py-2 pl-3 pr-4 text-neutral-900 rounded hover:bg-neutral-100 md:hover:bg-transparent md:hover:text-neutral-700 md:p-0 md:dark:hover:text-neutral-500 dark:text-white dark:hover:bg-neutral-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-neutral-700"
            >Contact</a
          >
        </li>
      </ul>
    </div>
  </div>
</nav>

<div class="flex justify-center items-center h-screen">
  <div class="w-3/4 h-3/4 rounded-lg dark:bg-emerald-700">
    <div class="dark:bg-emerald-400 rounded-lg flex justify-center items-center">
      <WheyTable />
    </div>
  </div>
</div>


<footer class="flex justify-center items-center">
  <div class="">
    <p class="dark:text-white">&copy; 2023 Nick Strijbos. All rights reserved.</p>
  </div>
</footer>