<script lang="ts">
    import MainNav from '$lib/components/layout/main-nav.svelte';
    import Footer from '$lib/components/landing/footer.svelte';
    import { Card, CardHeader, CardTitle, CardContent, CardDescription } from '$lib/components/ui/card/index.js';
    import { Calendar, Zap, Clock, Activity } from 'lucide-svelte'; // icons for each step
  </script>
  
  <MainNav />
  
  <main class="min-h-screen p-6 flex flex-col items-center gap-8 max-w-6xl mx-auto">
    <h1 class="text-3xl font-bold text-center">How to Use FITT</h1>
  
    <p class="text-center text-gray-700 max-w-3xl">
      You can use FITT by first setting the frequency you want to exercise; this will help you be consistent with your schedule. 
      Second, set the intensity; this will be personalised to your level of fitness, gradually increasing as you progress. 
      Third, determine the duration of your workouts; starting with shorter sessions is fine, gradually increasing as you get fitter. 
      Fourth, choose exercises that match your goals, for example cardio, strength, flexibility, or a mix of these.
    </p>
  
    <section class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-2 gap-6 w-full mt-6">
      <!-- Step 1: Frequency -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Calendar class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Step 1: Set Frequency</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            Decide how many times per week you’ll exercise to stay consistent with your schedule.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Step 2: Intensity -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Zap class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Step 2: Choose Intensity</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            Pick a challenging but safe effort level for each session. Gradually increase as you progress.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Step 3: Time -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Clock class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Step 3: Determine Time</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            Decide the duration of each workout. Start with shorter sessions if needed and increase as you get fitter.
          </CardDescription>
        </CardContent>
      </Card>
  
      <!-- Step 4: Type -->
      <Card class="text-center p-4">
        <CardHeader class="flex flex-col items-center">
          <Activity class="w-12 h-12 text-primary mb-2"/>
          <CardTitle>Step 4: Select Type</CardTitle>
        </CardHeader>
        <CardContent>
          <CardDescription>
            Choose exercises that match your goals: cardio, strength, flexibility, or a mix of these.
          </CardDescription>
        </CardContent>
      </Card>
    </section>
  
    <!-- Conclusion -->
    <p class="text-center text-gray-700 max-w-3xl mt-6">
      By following these four steps, FITT helps you long term to keep yourself motivated and consistent with your workouts.
    </p>
  </main>
  
  <Footer />
  