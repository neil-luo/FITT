<script lang="ts">
    import MainNav from '$lib/components/layout/main-nav.svelte';
    import Footer from '$lib/components/landing/footer.svelte';
    import { Card, CardHeader, CardTitle, CardContent, CardDescription } from '$lib/components/ui/card/index.js';
    import { Repeat, TrendingUp, Scale } from 'lucide-svelte'; // icons for each card
  </script>
  
  <MainNav />
  
  <main class="min-h-screen p-6 flex flex-col items-center gap-8 max-w-6xl mx-auto">
    <h1 class="text-3xl font-bold text-center">Why FITT is Important</h1>
  
    <p class="text-center text-gray-700 max-w-3xl">
      FITT is important because it helps you maintain consistency, ensures steady progression, 
      and encourages balance according to your current skill level.
    </p>
  
    <section class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 w-full mt-6">
      <!-- Consistency Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Repeat class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Consistency</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            FITT helps you stick to a schedule allowing you to be consistent with your workouts and achieving your goals consistently.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Progression Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <TrendingUp class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Progression</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            FITT allows you to progress at your own pace consistently allowing you to achieve your goals.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Balance Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Scale class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Balance</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            FITT enforces a level of balance, allowing yourself to avoid burn out and to stay consistent and progressing.
          </CardDescription>
        </CardContent>
      </Card>
    </section>
  
    <p class="text-center text-gray-700 max-w-3xl mt-6">
      By using FITT, you can be consistent, improving, and avoiding burn out.
    </p>
  </main>
  
  <Footer />
  