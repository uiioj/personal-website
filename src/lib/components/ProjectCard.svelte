<script lang="ts">

    export let title: string;
    export let subtitle: string;
</script>

<div class="bg-secondary text-secondary-foreground shadow-xl flex flex-col gap-4 justify-between">
	<div class="flex flex-col gap-16 pt-8">
		<div class="flex flex-col min-w-32 border-s-8 border-primary ps-8">
			<span class="font-bold text-primary text-xl">{title}</span>
			<span>{subtitle}</span>
		</div>
        </div>
        </div>
