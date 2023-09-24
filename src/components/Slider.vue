<template lang="">
    <div>
       
            <button @click="previous">Назад</button>
            <Slide :slide="sliders[num]"></Slide>
            <button @click="next">Вперед</button>
       
    </div>
</template>
<script>
import Slide from './Slide.vue'
export default {
    components: {
        Slide
    },
    data() {
        return {
            num: 0,
            sliders: [
                { title: 'Slider 1', text: 'some text 1' },
                { title: 'Slider 2', text: 'some text 2' },
                { title: 'Slider 3', text: 'some text 3' },
            ]
        }
    },
    methods: {
        previous() {
            if (this.num > 0) {
                this.num--;
            }
        },
        next() {
            if (this.num < this.sliders.length - 1) {
                this.num++;
            }
        }
    }
}
</script>
<style lang="">
    
</style>