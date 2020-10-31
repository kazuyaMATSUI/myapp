<template>
    <div id="thumbnails">
            <!-- <video width="400" height="400" v-for="item in items" v-bind:key="item.id">
                <source src="item.url">
            </video> -->
            <!-- <video width="400" height="400" autoplay src="@/assets/v3.mp4">
            </video> -->
            <video class="video" width="400" height="400" 
            v-for="item in items" 
            v-bind:key="item.id" 
            v-bind:autoplay="true" 
            v-bind:src="item.url"
            v-bind:loop="true"
            v-bind:muted="true"
            v-bind:playsinline="true"
            ></video>
    </div>
</template>

 
<script>
    export default {
        data: () => ({
            items: [
                { id: 1, url: 'https://player.vimeo.com/external/459802291.sd.mp4?s=c846c0ef9292600014ca216aa0be31496974e3a6&profile_id=164', played:"true"},
                { id: 2, url: 'https://player.vimeo.com/external/407595474.sd.mp4?s=8a9ad9ea95d9c5f7099e861281650808f1a63c56&profile_id=164', played:"false"},
                { id: 3, url: 'https://player.vimeo.com/external/441301097.sd.mp4?s=e97e70d51f93106825958d1a232db985f8844fba&profile_id=164', played:"false"},
                { id: 4, url: 'https://player.vimeo.com/external/449623829.hd.mp4?s=82893a1e42c7c1b177128a86a6253b7c4d1f071f&profile_id=174', played:"false"},
                { id: 5, url: 'https://player.vimeo.com/external/413229662.hd.mp4?s=26815ea7e1ba43aa54042b394780fbde2ad33d02&profile_id=174', played:"false"},
            ]
        }),
        // method: ()=>({
        //     play: function(event){
        //         this.played=true;
        //     }
        // })
    }
</script>
