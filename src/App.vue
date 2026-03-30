<script setup lang="ts">
import { NText, NH1, NDivider, NInfiniteScroll, NBlockquote, NCard, NFlex, NP } from 'naive-ui'
import LOGO from './assets/main_logo.svg'
import ICON from './assets/icon.svg'
</script>

<template>
    <div class="slide center" style="background-color: white">
        <img :src="LOGO" style="width: 60vw" />
        <NH1><NText code style="font-size: 1.75vw">Website of Unknown</NText> </NH1>
    </div>
    <NDivider />
    <div
        class="slide"
        style="background-color: white; align-content: center; justify-items: center"
    >
        <NCard hoverable bordered style="min-width: 10vw; max-width: fit-content">
            <NFlex>
                <div style="display: flex">
                    <img style="height: 10vw" :src="ICON" />
                    <NDivider style="height: 10vw" vertical />

                    <NText style="align-content: center; margin-left: 1vw">
                        <ruby>未完成<rt>みかんせい</rt></ruby>
                        の<ruby>可能性<rt>かのうせい</rt></ruby> <ruby>今日<rt>きょう</rt></ruby
                        >の<strong>アーカイブ</strong>に<ruby>残<rt>のこ</rt></ruby
                        >したい <br />
                        いつかきっと<ruby>未来<rt>みらい</rt></ruby
                        >の<ruby>私<rt>わたし</rt></ruby
                        >と<ruby>答<rt>こた</rt></ruby
                        >え<ruby>合<rt>あ</rt></ruby
                        >わせしよう
                        <br />
                        <NText italic depth="3" style="justify-self: right; font-size: 1vw"
                            >——Clear Morning</NText
                        >
                    </NText>
                </div>
            </NFlex>
        </NCard>
    </div>
    <NDivider />
    <div class="slide" style="background-color: white"></div>
</template>

<style>
* {
    font-size: 1.5vw;
}
rt {
    font-size: 1vw;
}

html,
body,
#app {
    scroll-snap-type: x mandatory;
}
body {
    margin: 0;
    min-height: 100vh;
    /* padding-left: 0.5rem;
    padding-right: 0.5rem; */
}
.center {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    user-select: none;
}
.slide {
    scroll-snap-align: center;
    min-height: 100vh;
}
</style>
