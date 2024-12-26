<script>

export default {
  data() {
    return {
        links:[
            {
                label:'Home',
                url:''
            },
            {
                label:'Piloti',
                url:''
            },
            {
                label:'Costruttori',
                url:''
            },
            {
                label:'Circuiti',
                url:''
            },
            {
                label:'Stagione',
                url:''
            },
            {
                label:'Risultati',
                url:''
            },
        ]
    }
  },

  components:{

  },

  methods: {

  }
}
</script>

<template> 
    <nav class="relative flex flex-wrap justify-between px-5 py-10 gap-20 items-center h-full">
        <ul class="flex gap-10 flex-wrap items-center">
            <li class="text-gray-400 transition-all ease-in-out duration-200 hover:translate-x-5 hover:text-white font-kanit w-full text-7xl" v-for="(link, index) in links" :key="index">
                <button class="uppercase relative font-semibold">
                        {{ link.label }}
                        <div class="absolute inset-0 pointer-events-none z-20">
                            <div class="w-full h-full bg-gradient-to-l from-black via-black/50 to-transparent"></div>
                        </div>
                </button>
            </li>
        </ul>
    </nav>
</template>

<style scoped>

</style>

