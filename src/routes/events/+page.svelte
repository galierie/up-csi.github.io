<script>
    import events, { Tag } from '$lib/data/events';
    import FeaturedEvent from '$lib/components/headers/FeaturedEvent.svelte';
    import FilterPagePanel from '$lib/components/panels/FilterPagePanel.svelte';
    import lino from '$lib/assets/lino/lino-sablay.svg';

    const filters = [
        'All',
        'EX Series',
        'App Process',
        'General Assembly',
        'Partnership',
        'Workshop',
        'Other',
    ];
</script>

<article class="prose dark:prose-invert flex max-w-full flex-col gap-8">
    <FeaturedEvent tags={[Tag.App]} schedule={['']}>
        {#snippet image()}
            <img src={lino} alt="Incoming App Process" />
        {/snippet}
        {#snippet name()}
            Incoming App Process...
        {/snippet}
        {#snippet description()}
            Stay Tuned...
        {/snippet}
    </FeaturedEvent>
    <FilterPagePanel {filters} cardsInfo={events} />
</article>
