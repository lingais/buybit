<script>

import {onMount} from "svelte";
import ky from 'ky';
import metagrabber from "meta-grabber"


let data;
onMount(async ()=>{
    const meta = metagrabber

    // const json = await ky.post('https://preview-grabber.vercel.app/api?url=https://www.youtube.com/watch?v=n48j6Yc2zWE&t=27s', {json: {foo: true}}).json();

    // console.log(json);
    console.log(meta("https://www.youtube.com/watch?v=EQy-AYhZIlE&t=370s"))

})

</script>


<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
