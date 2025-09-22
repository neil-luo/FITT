<script lang="ts">
    import MainNav from '$lib/components/layout/main-nav.svelte';
    import Footer from '$lib/components/landing/footer.svelte';
    import { Card, CardHeader, CardTitle, CardContent, CardDescription } from '$lib/components/ui/card/index.js';
    import { Calendar, Zap, Clock, Activity } from 'lucide-svelte';
  </script>
  
  <MainNav />
  
  <main class="min-h-screen p-6 flex flex-col items-center gap-8 max-w-6xl mx-auto">
    <h1 class="text-3xl font-bold text-center">About FITT</h1>
  
    <p class="text-center text-gray-700 max-w-3xl">
      FITT is about helping yourself organise and prevent burnout. It allows you to settle on a structured way of exercising and keep yourself fit. It includes:
    </p>
  
    <section class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 w-full mt-6">
      <!-- Frequency Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Calendar class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Frequency</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            This is how often you exercise. Be consistent and you'll get your expected results.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Intensity Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Zap class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Intensity</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            How much you want to challenge yourself. This is personal, tweak it to your own level.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Time Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Clock class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Time</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            How long an exercise session lasts. 30 minutes is recommended for most people; set it to what is best for you.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Type Card -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Activity class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Type</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            The kind of exercise you do, e.g., cardio, strength, or flexibility. A mix is recommended for most people.
          </CardDescription>
        </CardContent>
      </Card>
    </section>
  
    <p class="text-center text-gray-700 max-w-3xl mt-6">
      FITT is about organising yourself, preventing burnouts, and keeping yourself fit.
    </p>
  </main>
  
  <Footer />
  