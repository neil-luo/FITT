<script lang="ts">
    import { page } from '$app/stores';
    import { writable } from 'svelte/store';
    import { cn } from '$lib/utils.js';
    import {
      NavigationMenuRoot,
      NavigationMenuList,
      NavigationMenuItem
    } from '$lib/components/ui/navigation-menu/index.js';
  
    const activeSection = writable('');
  
    const normalizePath = (path: string) => path.replace(/\/$/, '');
  
    // Optional scroll tracking (for homepage sections)
    const handleScroll = () => {
      if (normalizePath($page.url.pathname) !== '') return;
      const featuresSection = document.getElementById('features');
      if (!featuresSection) return;
  
      const rect = featuresSection.getBoundingClientRect();
      activeSection.set(rect.top <= 100 && rect.bottom >= 100 ? 'features' : 'home');
    };
  
    $: currentPath = normalizePath($page.url.pathname);
  </script>
  
  <nav class="w-full backdrop-blur-sm flex items-center px-4 sm:px-6 lg:px-8 py-4">
    <!-- Desktop Navigation -->
    <div class="hidden lg:flex flex-1 justify-center">
      <NavigationMenuRoot>
        <NavigationMenuList class="flex space-x-6">
          <!-- Footer-linked pages -->
          <NavigationMenuItem>
            <a href="/about" class={cn(
              'font-medium hover:text-primary',
              currentPath === '/about' ? 'text-primary' : ''
            )}>
              About
            </a>
          </NavigationMenuItem>
  
          <NavigationMenuItem>
            <a href="/why" class={cn(
              'font-medium hover:text-primary',
              currentPath === '/why' ? 'text-primary' : ''
            )}>
              Why
            </a>
          </NavigationMenuItem>
  
          <NavigationMenuItem>
            <a href="/how" class={cn(
              'font-medium hover:text-primary',
              currentPath === '/how' ? 'text-primary' : ''
            )}>
              How
            </a>
          </NavigationMenuItem>
  
          <NavigationMenuItem>
            <a href="/when" class={cn(
              'font-medium hover:text-primary',
              currentPath === '/when' ? 'text-primary' : ''
            )}>
              When
            </a>
          </NavigationMenuItem>
  
          <NavigationMenuItem>
            <a href="/how-to" class={cn(
              'font-medium hover:text-primary',
              currentPath === '/how-to' ? 'text-primary' : ''
            )}>
              How-to
            </a>
          </NavigationMenuItem>
  
        </NavigationMenuList>
      </NavigationMenuRoot>
    </div>
  </nav>
  