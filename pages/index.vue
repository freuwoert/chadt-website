<template>
    <HeSection id="home">
        <HeLimiter size="text">
            <HeFlex class="hero" align-x="center">
                <h1 class="m-0 text-center text-lime-400 text-5xl leading-snug font-semibold">Chilln' auf der Tanke</h1>
                <h1 class="m-0 text-center text-zinc-200 text-3xl leading-normal font-normal">» Catered Rave im Lost Place «</h1>
                <HeFlex horizontal gap="1rem" padding="2rem 0 0">
                    <IodButton is="a" size="l" corner="pill" label="Sei jetzt dabei" shadow="l" background="var(--bg-lime-400)" target="_blank" href="https://calendar.app.google/XmvWRP3xdMFNfaKJ6"/>
                    <IodButton is="a" size="l" corner="pill" label="Mehr erfahren" border shadow="l" variant="contained" background="var(--bg-lime-400)" href="/#about"/>
                </HeFlex>
            </HeFlex>
        </HeLimiter>
        <template #background>
            <img class="h-full w-full absolute inset-0 object-cover" src="/images/hero.jpg">
            <div class="h-full w-full absolute inset-0 bg-zinc-900 opacity-80"></div>
        </template>
    </HeSection>

    <HeSection divider-position="absolute-outer" id="about">
        <HeLimiter>
            <HeFlex padding="6rem 0" gap="4rem">
                <HeFlex horizontal gap="2rem 4rem" align-y="flex-start" breakpoint="768">
                    <div class="flex-1">
                        <img src="/images/about.png" class="flex-1 rounded-xl aspect-video"/>
                    </div>
                    <div class="flex-1">
                        <h2 class="m-0 text-lime-400 text-4xl leading-snug font-semibold">Über CHADT</h2>
                        <h3 class="m-0 mb-6 text-zinc-200 text-2xl leading-snug font-normal italic">Was is Chilln' auf der Tanke überhaupt?</h3>
                        <p class="mb-4">
                            Was als kleine Geburtstagsfeier in einem Lost Place bei Salzgitter angefangen hat, hat sich schnell zu einem Outdoor Rave samt Catering weiterentwickelt.
                            Mit Chilln' auf der Tanke möchte ich die entspannten Summer Vibes eines Gartenfests mit dem Kick von Lost Places kombinieren.
                        </p>
                        <p class="mb-4">
                            Egal ob Turn Up oder Chill Out, die einzigartige Location hat Chilln' auf der Tanke schon letztes Jahr zu einem unvergesslichen Erlebnis gemacht.
                        </p>
                    </div>
                </HeFlex>
            </HeFlex>
        </HeLimiter>

        <template #above>
            <HeShapeDivider shape="arrow" height="2rem" background="var(--bg-zinc-900)" inverted flip-x/>
        </template>
    </HeSection>



    <HeSection divider-position="absolute-outer" background="var(--bg-zinc-800)" id="when-and-where">
        <HeLimiter>
            <HeFlex padding="6rem 0" gap="4rem">
                <HeFlex horizontal gap="2rem 4rem" align-y="flex-start" breakpoint="768" reversed>
                    <iframe
                        class="flex-1 aspect-video rounded-xl"
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d363.94878376349305!2d10.414229456996376!3d52.14622035827743!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47a55a31f9578ebf%3A0xc4100315ba66210e!2sAm%20Gummibahnhof%209%2C%2038239%20Salzgitter!5e0!3m2!1sen!2sde!4v1716217824966!5m2!1sen!2sde"
                        allowfullscreen
                        loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                    <div class="flex-1">
                        <h2 class="m-0 text-lime-400 text-4xl leading-snug font-semibold">Wann und Wo</h2>
                        <h3 class="m-0 mb-6 text-zinc-200 text-2xl leading-snug font-normal italic">Wann findet's statt und wo muss ich sein?</h3>
                        <p class="mb-4">
                            Angepeilt ist der <b>Samstag, 06. Juli 2024</b> ab ca. <b>15:00 Uhr</b>.<br>
                            Die Location ist der <a href="https://maps.app.goo.gl/FxXNxfyXZyxGEMTt5" target="_blank"><b>Gummibahnhof 9 in Salzgitter</b></a>¹.
                        </p>
                        <p class="mb-6">
                            Da die Location mit ÖPNV nicht all zu gut zu erreichen ist, empfehlen wir Fahrgemeinschaften. Parkplätze sind ausreichend vorhanden.
                            Fragt mich auch gerne persönlich, wenn ihr eine Mitfahrgelegenheit sucht.
                        </p>
                        <IodButton is="a" label="Sei jetzt dabei" href="https://calendar.app.google/XmvWRP3xdMFNfaKJ6" target="_blank" corner="pill" background="var(--bg-lime-400)"/>
                    </div>
                </HeFlex>
            </HeFlex>
        </HeLimiter>

        <template #above>
            <HeShapeDivider shape="arrow" height="2rem" background="var(--bg-zinc-800)" inverted/>
        </template>
    </HeSection>



    <HeSection divider-position="absolute-outer" id="fee">
        <HeLimiter>
            <HeFlex padding="6rem 0" gap="4rem">
                <HeFlex horizontal gap="2rem 4rem" align-y="flex-start" breakpoint="768">
                    <div class="flex-1">
                        <img src="/images/about.png" class="flex-1 rounded-xl aspect-video"/>
                    </div>
                    <div class="flex-1">
                        <h2 class="m-0 text-lime-400 text-4xl leading-snug font-semibold">Eintritt</h2>
                        <h3 class="m-0 mb-6 text-zinc-200 text-2xl leading-snug font-normal italic">Das kostet Geld!?</h3>
                        <p class="mb-4">
                            Natürlich verlange ich <b>keinen Eintritt</b> für meine Geburtstagsfeier.
                            Da ich euch alle mit Catering und Getränken versorgen möchte, ist ein kleines, geldliches <b>Geburtstagsgeschenk (15-20€)</b> aber immer gerne gesehen.
                        </p>
                    </div>
                </HeFlex>
            </HeFlex>
        </HeLimiter>

        <template #above>
            <HeShapeDivider shape="arrow" height="2rem" background="var(--bg-zinc-900)" inverted flip-x/>
        </template>
    </HeSection>



    <HeSection divider-position="absolute-outer" background="var(--bg-zinc-800)" id="faq">
        <HeLimiter>
            <HeFlex padding="6rem 0">
                <h2 class="m-0 text-lime-400 text-4xl leading-snug font-semibold">FAQ</h2>
                <h3 class="m-0 mb-6 text-zinc-200 text-2xl leading-snug font-normal italic">Was muss ich sonst noch wissen?</h3>
                <IodAccordion title="Ist das legal?" class="rounded-xl mb-2">
                    <p class="px-4 pb-4">
                        Ja, Chilln' auf der Tanke ist eine private Geburtstagsfeier. Die Location ist ein öffentlicher Lost Place ohne Zugangsschutz und somit legal zu betreten.
                        Das Tankstellengebäude ist jedoch nicht begehbar und wird auch nicht betreten.
                    </p>
                </IodAccordion>
                <IodAccordion title="Was muss ich mitbringen?" class="rounded-xl mb-2">
                    <p class="px-4 pb-4">
                        Die Empfehlungen sind: <b>Picknickdecke, Sonnencreme und Mückenspray</b>.
                        Ich werde mich um das Catering und einige alkoholische und nicht-alkoholische Getränke kümmern. Wer möchte, kann aber auch gerne etwas zum Teilen mitbringen. #BYOB
                    </p>
                </IodAccordion>
                <IodAccordion title="Geburtstagsgeschenk?" class="rounded-xl mb-2">
                    <p class="px-4 pb-4">
                        Da ich euch alle mit Catering und Getränken versorgen möchte, ist ein kleines, geldliches <b>Geburtstagsgeschenk (15-20€)</b> aber immer gerne gesehen.
                    </p>
                </IodAccordion>
                <IodAccordion title="Gibt es eine Toilette?" class="rounded-xl mb-2">
                    <p class="px-4 pb-4">
                        <b>Leider nein!</b>
                        Da die Location ein Lost Place ist, gibt es keine sanitären Anlagen.
                        Ich versuche jedoch einen Wasserkanister zu organisieren.
                        Bitte plant das bei eurer Anreise ein.
                    </p>
                </IodAccordion>
                <IodAccordion title="Wie siehts mit Parkplätzen aus?" class="rounded-xl mb-2">
                    <p class="px-4 pb-4">
                        Parkplätze sind ausreichend vorhanden. Da die Location mit ÖPNV nicht all zu gut zu erreichen ist, empfehlen wir Fahrgemeinschaften.
                        Fragt mich auch gerne persönlich, wenn ihr eine Mitfahrgelegenheit sucht.
                    </p>
                </IodAccordion>
                <IodAccordion title="Wie lange geht die Party?" class="rounded-xl mb-2">
                    <p class="px-4 pb-4">
                        Geplant ist ein entspannter Nachmittag, Abend und Nacht. Geht mal von 2:00-3:00 Uhr aus.
                    </p>
                </IodAccordion>
                <IodAccordion title="Was ist, wenn es regnet?" class="rounded-xl mb-2">
                    <p class="px-4 pb-4">
                        Da Chilln' auf der Tanke ein Outdoor-Event ist, kann es bei schlechtem Wetter auch mal ins Wasser fallen.
                        Ich versuche jedoch ein Pavillon zu organisieren für alle Fälle.
                    </p>
                </IodAccordion>
            </HeFlex>
        </HeLimiter>

        <template #above>
            <HeShapeDivider shape="arrow" height="2rem" background="var(--bg-zinc-800)" inverted/>
        </template>
    </HeSection>
</template>

<style lang="sass" scoped>
    .hero
        min-height: 60vh
</style>