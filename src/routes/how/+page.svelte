<script lang="ts">
    import MainNav from '$lib/components/layout/main-nav.svelte';
    import Footer from '$lib/components/landing/footer.svelte';
    import { Card, CardHeader, CardTitle, CardContent, CardDescription } from '$lib/components/ui/card/index.js';
    import { CheckCircle, Calendar, Zap } from 'lucide-svelte'; // icons for each card
  </script>
  
  <MainNav />
  
  <main class="min-h-screen p-6 flex flex-col items-center gap-8 max-w-6xl mx-auto">
    <h1 class="text-3xl font-bold text-center">How FITT Helps You</h1>
  
    <p class="text-center text-gray-700 max-w-3xl">
      FITT can help you achieve your fitness goals by enforcing consistency, organisation, and by helping you avoid burnout.
    </p>
  
    <section class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 w-full mt-6">
      <!-- Consistency Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <CheckCircle class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Consistency</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            Consistency allows you to achieve your goals without a surprise, while also making your day more scheduled.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Organisation Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Calendar class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Organisation</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            FITT can organise your day by allowing you to schedule ahead of time, which lets you plan effectively.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Burning Out Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Zap class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Burning Out</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            FITT enforces a balance of intensity and time, allowing you to personalise your exercises without burning out.
          </CardDescription>
        </CardContent>
      </Card>
    </section>
  
    <p class="text-center text-gray-700 max-w-3xl mt-6">
      By applying FITT, you can structure your workouts to be consistent, organised, and easy to follow.
    </p>
  </main>
  
  <Footer />
  