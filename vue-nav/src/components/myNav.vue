<template>
    <nav v-bind:class="active">
        <a class="home" v-on:click="select('home')" href="#">home</a>
        <a class="projects" v-on:click="select('projects')" href="#">projects</a>
        <a class="services" v-on:click="select('services')" href="#">services</a>
        <a class="contact" v-on:click="select('contact')" href="#">contact</a>
    </nav>
</template>
<script>
export default {
    data () {
        return {
            active: 'home'
        }
    },
    methods: {
        select: function(item){
            this.active = item
            console.log('click: '+item);
        }
    }
}
</script>
<style>
	nav{
		font:15px/1.3 'Open Sans', sans-serif;
		text-align:center;
        width: 100%;
        background-color: #068bbb;
	}

	nav a{
		display:inline-block;
		padding: 18px 30px;
		color:#fff !important;
		font-weight:bold;
		font-size:16px;
		text-decoration:none !important;
		line-height:1;
		text-transform: uppercase;
		background-color:transparent;
	}

    a:hover{
        background-color: #096c9e;
	}
	.home .home,            /*第一个值是nav的，第二个值是a标签的*/
	.projects .projects,
	.services .services,
	.contact .contact{
		background-color:#e35885;
	}
</style>