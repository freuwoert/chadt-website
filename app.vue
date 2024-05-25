<template>
    <HeSection is="header" class="border-b border-b-zinc-800" shadow="l" sticky divider-position="absolute-outer">
        <HeLimiter>
            <HeFlex class="h-16" horizontal gap="1rem">
                <HeLogo href="/" src="/images/logo.png" alt="Logo Ipsum"/>
                <HeSpacer />
                <HeMenu :menu="menu" mobile-submenu-show-toggle />
                <IodButton is="a" size="s" corner="pill" label="Sei dabei" background="var(--bg-lime-400)" target="blank" href="https://calendar.app.google/XmvWRP3xdMFNfaKJ6"/>
            </HeFlex>
        </HeLimiter>
    </HeSection>

    <main>
        <NuxtPage />
    </main>

    <HeSection class="border-t border-t-zinc-800" is="footer">
        <HeLimiter>
            <HeFlex class="min-h-16" padding="1rem 0" horizontal gap="1rem 2rem" breakpoint="768">
                <small>© {{ new Date().getFullYear() }} Alyx Freuwört</small>
                <HeSpacer class="hidden md:flex"/>
                <small><NuxtLink to="/legal">Impressum und Datenschutz</NuxtLink></small>
            </HeFlex>
        </HeLimiter>
    </HeSection>
</template>

<script lang="ts" setup>
    useHead({
        htmlAttrs: {
            lang: 'de',
        }
    })
    const menu = ref([
        { id: 'home', label: 'Home', href: '/' },
        { id: 'about', label: 'Über CHADT', href: '/#about' },
        { id: 'when-and-where', label: 'Wann und Wo', href: '/#when-and-where' },
        { id: 'fee', label: 'Eintritt', href: '/#fee' },
        { id: 'faq', label: 'FAQ', href: '/#faq' },
    ])
</script>

<style lang="sass" scoped>
    header
        background-color: var(--bg-zinc-900)
        background-image: url('/images/grunge.jpg') !important
        background-size: cover
        background-position: top center
        background-blend-mode: screen
</style>