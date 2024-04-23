<script>
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
  </script>

<Navbar  >
    <NavBrand href="/">
      
      <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Jacob's Projects</span>
    </NavBrand>
    <NavHamburger  />
    <NavUl >
      <NavLi href="/about">About Me</NavLi>
      
      <NavLi href="/contact">Contact</NavLi>
    </NavUl>
  </Navbar>
  
  