<script lang="ts">
    import { Card, CardContent, CardHeader, CardTitle, CardDescription } from '$lib/components/ui/card/index.js';
    import { Button } from '$lib/components/ui/button/index.js';
    import MainNav from '$lib/components/layout/main-nav.svelte';
    import Footer from '$lib/components/landing/footer.svelte';
  </script>  
  
  <MainNav />
  <main class="min-h-screen bg-gray-50 flex flex-col items-center p-6">
    <!-- Hero Section -->
    <section class="text-center max-w-3xl mb-16">
      <h1 class="text-4xl font-bold mb-4">FITT Principle</h1>
      <p class="text-lg text-gray-700">
        Learn how to structure your exercise routine for maximum results. FITT stands for Frequency, Intensity, Time, and Type.
      </p>
      <Button class="mt-6" on:click={() => alert('Start your journey!')}>Get Started</Button>
    </section>
  
    <!-- FITT Cards -->
    <section class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 w-full max-w-6xl">
      <Card>
        <CardHeader>
          <CardTitle>Frequency</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            How often you exercise. Consistency is key to progress.
          </CardDescription>
        </CardContent>
      </Card>
  
      <Card>
        <CardHeader>
          <CardTitle>Intensity</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            How hard you exercise. Challenge yourself but stay safe.
          </CardDescription>
        </CardContent>
      </Card>
  
      <Card>
        <CardHeader>
          <CardTitle>Time</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            How long each session lasts. Balance duration with intensity.
          </CardDescription>
        </CardContent>
      </Card>
  
      <Card>
        <CardHeader>
          <CardTitle>Type</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            The kind of exercise you do. Mix cardio, strength, and flexibility.
          </CardDescription>
        </CardContent>
      </Card>
    </section>
  
    <!-- CTA Section -->
    <section class="mt-16 text-center max-w-3xl">
      <h2 class="text-2xl font-semibold mb-4">Ready to improve your fitness?</h2>
      <p class="text-gray-600 mb-6">
        Apply the FITT principle to your workouts and see results faster. Start today!
      </p>
      <Button on:click={() => alert('Time to sweat!')}>Start Training</Button>
    </section>
  </main>
  <Footer />
  
  <style>
    main {
      font-family: system-ui, sans-serif;
    }
  </style>
  