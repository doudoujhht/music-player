<script>
    let classes= "w-full border-b-[1px] border-[rgb(255,255,255,0.3)] cursor-pointer "
    export let image;
    export let titre;
    export let artiste;
    
</script>
<div class={classes}>
	<div
		class="flex items-center gap-5 bg-[rgb(255,255,255,0.2)] p-5 text-white"
	>
		<img
			src={image}
			alt=""
			class="w-12 h-12 rounded-full"
		/>
		<div class="w-[13rem]">
			<h1 class="font-bold">{titre}</h1>
            <p>{artiste}</p>
		</div>
	</div>
</div>