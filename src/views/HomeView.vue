<script setup>
import EventCard from '@/components/EventCard.vue';
import { ref } from 'vue';

const events = ref([
    {
  id:5928101,
  category:'Animal Welfare',
  title:'Cat Adoption day',
  description:'Find your feline friend from this event',
  location:'meow town',
  date:'January 28,2025',
  time:'12:00',
  petsAllowed:true,
  organizer:'Kat Laydee'
},
  {
  id:4567890,
  category:'Food',
  title:'Community Gardening',
  description:'Find your feline friend from this event',
  location:'Flora City',
  date:'March 16,2025',
  time:'10:00',
  petsAllowed:true,
  organizer:'Kat Laydee'
},
  {
  id:7689564,
  category:'Sustainability',
  title:'Beach Cleanup',
  description:'Find your feline friend from this event',
  location:'Marine drive',
  date:'August 24,2025',
  time:'14:00',
  petsAllowed:true,
  organizer:'Kat Laydee'
},

])
</script>

<template>
 <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event"/>
 </div>
</template>

<style scoped>
.events{
    display: flex;
    flex-direction: column;
    align-items: center;
}
</style>
