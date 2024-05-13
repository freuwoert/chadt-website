<template>
    <HeSection is="header" height="4rem" background="var(--bg-zinc-800)" sticky divider-position="absolute-outer">
        <HeLimiter>
            <HeFlex class="h-16" horizontal gap="1rem">
                <HeLogo href="/" src="https://img.logoipsum.com/288.svg" alt="Logo Ipsum"/>
                <HeSpacer />
                <HeMenu :menu="menu" mobile-submenu-show-toggle />
            </HeFlex>
        </HeLimiter>
        <template #below>
            <HeShapeDivider shape="triangle" height=".75rem" background="var(--bg-zinc-800)"  flip-x/>
        </template>
    </HeSection>

    <HeSection background="var(--bg-zinc-900)">
        <HeLimiter>
            <HeFlex horizontal padding="4rem 0" gap="2rem" breakpoint="768" reversed>
                <HeFlex class="flex-1">
                    <IodCarousel dots arrows infinite :interval="5000" overlay class="h-80 rounded-xl">
                        <template #slide-1>
                            <Visualizer />
                        </template>
                        <template #slide-2>
                            <Visualizer />
                        </template>
                    </IodCarousel>
                </HeFlex>
                <HeFlex class="flex-1">
                    <h1 class="m-0 text-lime-400">Iodine + Helium</h1>
                    <p>
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eligendi ipsum praesentium dignissimos dolorem
                        perferendis sequi aut exercitationem deserunt eos ratione asperiores excepturi quaerat non cum alias ab, qui
                        numquam eius!
                    </p>
                </HeFlex>
            </HeFlex>
        </HeLimiter>
        <template #below>
            <HeShapeDivider shape="triangle" height="2rem" background="var(--bg-zinc-900)"/>
        </template>
    </HeSection>

    <HeSection>
        <HeLimiter>
            <HeFlex padding="4rem 0" gap="4rem">
                <HeFlex horizontal gap="2rem 4rem" align-y="flex-start" breakpoint="768">
                    <Visualizer class="flex-1 rounded-xl aspect-video"/>
                    <div class="flex-1">
                        <h2>Section 1</h2>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eligendi ipsum praesentium dignissimos
                            dolorem perferendis sequi aut exercitationem deserunt eos ratione asperiores excepturi quaerat non.
                        </p>
                    </div>
                </HeFlex>
                <HeFlex horizontal gap="2rem 4rem" align-y="flex-start" breakpoint="768" reversed>
                    <Visualizer class="flex-1 rounded-xl aspect-video"/>
                    <div class="flex-1">
                        <h2>Section 1</h2>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eligendi ipsum praesentium dignissimos
                            dolorem perferendis sequi aut exercitationem deserunt eos ratione asperiores excepturi quaerat non.
                        </p>
                    </div>
                </HeFlex>
            </HeFlex>
        </HeLimiter>
    </HeSection>

    <footer>
        <HeSection is="div" background="var(--bg-zinc-900)">
            <template #above>
                <HeShapeDivider shape="triangle" height=".75rem" background="var(--bg-zinc-900)" flip-y />
            </template>
            <HeLimiter>
                <HeFlex horizontal padding="4rem 0" gap="2rem" align-y="flex-start" breakpoint="768">
                    <HeFlex class="flex-1">
                        <h3 class="m-0 text-lime-400">Contact</h3>
                        <HeDivider class="my-4"/>
                        <NuxtLink to="/">Menu Item 1</NuxtLink>
                        <NuxtLink to="/">Menu Item 2</NuxtLink>
                        <NuxtLink to="/">Menu Item 3</NuxtLink>
                        <NuxtLink to="/">Menu Item 4</NuxtLink>
                    </HeFlex>
                    <HeFlex class="flex-1">
                        <h3 class="m-0 text-lime-400">About us</h3>
                        <HeDivider class="my-4"/>
                        <NuxtLink to="/">Menu Item 1</NuxtLink>
                        <NuxtLink to="/">Menu Item 2</NuxtLink>
                    </HeFlex>
                    <HeFlex class="flex-1">
                        <h3 class="m-0 text-lime-400">Resources</h3>
                        <HeDivider class="my-4"/>
                        <NuxtLink to="/">Menu Item 1</NuxtLink>
                        <NuxtLink to="/">Menu Item 2</NuxtLink>
                        <NuxtLink to="/">Menu Item 3</NuxtLink>
                        <NuxtLink to="/">Menu Item 4</NuxtLink>
                    </HeFlex>
                    <HeFlex class="flex-1">
                        <h3 class="m-0 text-lime-400">Legal</h3>
                        <HeDivider class="my-4"/>
                        <NuxtLink to="/">Menu Item 1</NuxtLink>
                        <NuxtLink to="/">Menu Item 2</NuxtLink>
                        <NuxtLink to="/">Menu Item 3</NuxtLink>
                    </HeFlex>
                </HeFlex>
            </HeLimiter>
        </HeSection>
        <HeSection is="div" background="var(--bg-lime-400)" style="--color-text: var(--bg-zinc-900); color: var(--bg-zinc-900);">
            <HeLimiter>
                <HeFlex horizontal class="h-16">
                    <small>© {{ new Date().getFullYear() }} Logo Ipsum</small>
                    <HeSpacer />
                    <IodIconButton icon-font="var(--font-brand)" is="a" href="#" target="_blank" variant="text" corner="pill" icon="&#62002;" aria-label="WhatsApp" />
                    <IodIconButton icon-font="var(--font-brand)" is="a" href="#" target="_blank" variant="text" corner="pill" icon="&#61805;" aria-label="Instagram" />
                    <IodIconButton icon-font="var(--font-brand)" is="a" href="#" target="_blank" variant="text" corner="pill" icon="&#61594;" aria-label="Facebook" />
                </HeFlex>
            </HeLimiter>
        </HeSection>
    </footer>
</template>

<script lang="ts" setup>
    const menu = ref([
        { id: 'home', label: 'Start', href: '/' },
        { id: 'get-started', label: 'Was', href: '/' },
        { id: 'components', label: 'Wann', href: '/' },
        { id: 'demo', label: 'Wo', href: '/' },
        { id: 'demo', label: 'RSVP', href: '/' },
    ])
</script>