<template>
    <section id="categories" class="py-16 scroll-mt-20 bg-white">
        <div class="container mx-auto px-4">

            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold text-amber-950 mb-3">
                    Explore Our Animals Collections
                </h2> 
                <p class="text-lg text-gray-800 max-w-2xl mx-auto">
                    Discover yours personalities
                </p>
            </div>

            <div class="grid grid-cols-1 sm: grid-cols-2 lg: grid-cols-3 gap-6">
                 <div v-for="(category, index) in categories" :key="index"
                        class="relative group overflow-hidden rounded-lg shadow-md 
                                        hover: shadow-lg transition-shadow duration-300"
                 >

                      <a :href="category.authorLink" target="_blank" rel="noopener noreferrer">
                          <div class="h-64 overflow-hidden">
                              <img :src="category.image" :alt="category.alt" class="w-full h-full 
                                  object-cover group-hover:scale-105 transition-transform duration-500"
                              >
                          </div>
                      </a>

                      <div v-if="category.authorDescription"
                           class="absolute top-0 left-0 right-0 p-2 text-center text-sm font-medium 
                                  text-white bg-black/50 transition-opacity duration-300 opacity-0 
                                  group-hover:opacity-100"
                      >
                          {{ category.authorDescription }}
                      </div>
                      
                      <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent 
                           to-transparent"
                      >
                           <div class="absolute bottom-0 left-0 p-6">
                                 <h3 class="text-xl font-semibold text-white">
                                     {{ category.title}}
                                 </h3>
                                 <p class="text-gray-200 mt-1">
                                     {{ category.description }}
                                 </p>
                           </div>
                      </div>

                 </div>
            </div>
        </div>
    </section>
</template>

<script setup>
    import { ref } from 'vue';
   import  product8  from '../assets/images/product8.png';
   import  product9  from '../assets/images/product9.png';
   import  product10  from '../assets/images/product10.png';
   import  product11  from '../assets/images/product11.png';
   import  product12  from '../assets/images/product12.png';
   import  product13  from '../assets/images/product13.png';

    const categories = ref([
        // Exemplo: 'authorLink' e 'authorDescription' adicionados ao item do "Leão"
        {
          image:product8, 
          title:"Swan’s Collection", 
          description:"Pink topaz swan", 
          alt:"Swan’s Collection",
          authorLink: '#', // Link de exemplo
          authorDescription: null,
        },
        {
          image:product9, 
          title:"Wing’s Collection", 
          description:"Tourmalian wings", 
          alt:"Wing’s Collection",
          authorLink: '#',
          authorDescription: null,
        },
        {
          image:product10, 
          title:"Heart’s Collection", 
          description:"Ruby heart", 
          alt:"Heart’s Collection",
          authorLink: '#',
          authorDescription: null,
        },
        {
          image:product11, 
          title:"Jellyfish’s Collection", 
          description:"Emerald jellyfish", 
          alt:"Jellyfish’s Collection",
          authorLink: 'https://xvcuritiba.com.br/', // Link do site do autor
          authorDescription: 'Link Leão Dakar', // Descrição do autor
        },
        {
          image:product12, 
          title:"Butterfly’s Collection", 
          description:"Crystal butterfly", 
          alt:"Butterfly’s Collection",
          authorLink: '#',
          authorDescription: null,
        },
        {
          image:product13, 
          title:"Galaxy’s Collection", 
          description:"Emerald galaxy", 
          alt:"Galaxy’s Collection",
          authorLink: '#',
          authorDescription: null,
        },
    ])
</script>
