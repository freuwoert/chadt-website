<template>
    <HeSection is="header" height="4rem" background="var(--bg-zinc-900)" shadow="l" sticky divider-position="absolute-outer">
        <HeLimiter>
            <HeFlex class="h-16" horizontal gap="1rem">
                <HeLogo href="/" src="/images/chillen_auf_der_tanke_logo.png" alt="Logo Ipsum"/>
                <HeSpacer />
                <HeMenu :menu="menu" mobile-submenu-show-toggle />
                <IodButton is="a" size="s" corner="pill" label="Sei dabei" background="var(--bg-lime-400)" target="blank" href="https://calendar.app.google/XmvWRP3xdMFNfaKJ6"/>
            </HeFlex>
        </HeLimiter>
        <template #below>
            <HeShapeDivider shape="triangle" height=".5rem" background="var(--bg-zinc-900)"  flip-x/>
        </template>
    </HeSection>

    <main>
        <NuxtPage />
    </main>

    <HeSection class="border-t border-t-zinc-800" is="footer" background="var(--bg-zinc-900)">
        <HeLimiter>
            <HeFlex class="min-h-16" padding="1rem 0" horizontal gap="1rem 2rem" breakpoint="768">
                <small>© {{ new Date().getFullYear() }} Alyx Freuwört</small>
                <HeSpacer />
                <NuxtLink to="/">Impressum und Datenschutz</NuxtLink>
            </HeFlex>
        </HeLimiter>
    </HeSection>
</template>

<script lang="ts" setup>
    const menu = ref([
        { id: 'home', label: 'Home', href: '/' },
        { id: 'about', label: 'Über CHADT', href: '/#about' },
        { id: 'when-and-where', label: 'Wann und Wo', href: '/#when-and-where' },
        { id: 'fee', label: 'Eintritt', href: '/#fee' },
        { id: 'faq', label: 'FAQ', href: '/#faq' },
    ])
</script>