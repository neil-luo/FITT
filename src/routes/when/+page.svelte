<script lang="ts">
    import MainNav from '$lib/components/layout/main-nav.svelte';
    import Footer from '$lib/components/landing/footer.svelte';
    import { Card, CardHeader, CardTitle, CardContent, CardDescription } from '$lib/components/ui/card/index.js';
    import { Play, TrendingUp } from 'lucide-svelte'; // icons for each card
  </script>
  
  <MainNav />
  
  <main class="min-h-screen p-6 flex flex-col items-center gap-8 max-w-6xl mx-auto">
    <h1 class="text-3xl font-bold text-center">When FITT Helps</h1>
  
    <p class="text-center text-gray-700 max-w-3xl">
      FITT helps when you're starting out and allows you to progress and organise your fitness life.
    </p>
  
    <section class="grid grid-cols-1 sm:grid-cols-2 gap-6 w-full mt-6">
      <!-- Starting Out Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Play class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Starting Out</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            FITT can help you when you're starting out by allowing you to stay consistent and progress as a beginner, making exercise easier to schedule.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Progressing Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <TrendingUp class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Progressing</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            FITT can not only help beginners; it can also help people looking to progress with different types of exercise and intensity.
          </CardDescription>
        </CardContent>
      </Card>
    </section>
  
    <p class="text-center text-gray-700 max-w-3xl mt-6">
      By applying FITT, you can structure your workouts for consistent improvement and long-term results.
    </p>
  </main>
  
  <Footer />
  