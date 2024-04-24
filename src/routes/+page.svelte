<script>
    import Appbar from "../lib/Appbar.svelte";
    import data from "../projects_description.json";
    export let items = data;
  
  </script>
  
  <main>
    
    <div class= "navbar">
      <Appbar />
    </div>
    <div class="p-8">
    </div>
     
    <div class="grid auto-cols-max grid-cols-1 md:grid-cols-1 lg:grid-cols-2 xl:grid-cols-2 ">
    {#each Object.values(items) as item}
      <div class="space-y-4 p-4">
        <a href={item.github} class="flex flex-col items-center bg-white rounded-lg shadow xl:flex-row lg:min-w-lg hover:bg-gray-100 dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
          <img class="object-cover w-full rounded-t-lg h-auto xl:w-96 md:rounded-none md:rounded-s-lg" src={item.path} alt="">
          <div class="flex flex-col justify-between p-2 leading-normal">
              <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"> {item.name}</h5>
              <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">{item.description}</p>
          </div>
        </a>
  
  
      </div>
     {/each}
  
    </div>
  
    
  </main>
  