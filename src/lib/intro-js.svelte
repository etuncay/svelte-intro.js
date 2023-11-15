<script lang="ts">
    import IntroJs from 'intro.js'
    import 'intro.js/minified/introjs.min.css'
    import {onMount} from 'svelte'
    
    export let options: any= {}
    onMount(() => {
        if(options!=null && options!.steps!=null && options!.steps!.length>0){
            for(let i=0; i<options!.steps!.length;i++){
                let step = options!.steps[i];
                if(step!.selector!=null){
                    options!.steps[i].element= document.querySelector(step!.selector);
                }
            } 
        }
        IntroJs().setOptions(options).start();
    });
</script>


<slot />