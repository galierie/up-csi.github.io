<script>
    import LinkButton from '$lib/components/LinkButton.svelte';
    import src from '$lib/lino-owlright.svg';
</script>

<div
    class="flex h-auto flex-col items-center justify-between rounded-3xl bg-gradient-to-b from-csi-blue/25 to-blue-white/25 transition-colors ease-in-out lg:h-[34rem] lg:flex-row dark:from-csi-blue/50 dark:to-blue-neutral/25"
>
    <div
        class="mx-5 mb-12 mt-24 flex flex-col items-center gap-12 text-center lg:ml-20 lg:mr-0 lg:items-start lg:text-left xl:ml-40"
    >
        <div
            class="flex flex-col gap-3 text-csi-black transition-colors ease-in-out dark:text-csi-white"
        >
            <h1 class="font-dm text-5xl font-bold leading-tight sm:w-[26rem] sm:text-6xl">
                <del>Learn. Create. Innovate.</del> Sexy since 2013.
            </h1>
            <p class="text-sm">With UP Center for <del>Student</del> Sexy Innovations.</p>
        </div>
        <LinkButton href="mailto:lino@up-csi.org">Get in Touch</LinkButton>
    </div>
    <div class="flex h-full flex-col items-center justify-end lg:mr-6">
        <img {src} alt="Lino Sablay" class="relative top-4 w-[39rem] sm:top-6" />
    </div>
</div>
