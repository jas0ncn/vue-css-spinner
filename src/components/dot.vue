<template>
    <div class="vue-css-spinner" v-show="loading">
        <div class="dot1" :style="[css, css1]"></div>
        <div class="dot2" :style="[css, css2]"></div>
        <div class="dot3" :style="[css, css3]"></div>
        <div class="dot4" :style="[css, css4]"></div>
    </div>
</template>

<script>
export default {
    name: 'dot',
    props: {
        loading: {
            type: Boolean,
            default: true
        },
        size: {
            type: Number,
            default: 10
        },
        color: {
            type: Array,
            default: function () {
                return ['#4285F4', '#DB4437', '#F4B400', '#0F9D58']
            }
        }
    },
    data () {
        return {
            css: {
                width: this.size + 'px',
                height: this.size + 'px'
            },
            css1: {
                background: this.color[0]
            },
            css2: {
                top: -this.size + 'px',
                background: this.color[1]
            },
            css3: {
                top: -this.size * 2 + 'px',
                background: this.color[2]
            },
            css4: {
                top: -this.size * 3 + 'px',
                background: this.color[3]
            }
        }
    }
}
</script>

<style lang="less" scoped>
@red: #4285F4;
@green: #DB4437;
@blue: #F4B400;
@yellow: #0F9D58;

* {
    margin: 0;
    padding: 0;
}
.dot {
    position: relative;
    left: 0;
    top: 0;
    opacity: 0;
    border-radius: 50%;
    animation: transform 3.5s infinite cubic-bezier(.2, .64, .81, .23);
}
.vue-css-spinner {
    width: 100%;
    overflow-x: hidden;
    .dot1 {
        .dot;
    }
    .dot2 {
        .dot;
        animation-delay: 200ms;
    }
    .dot3 {
        .dot;
        animation-delay: 400ms;
    }
    .dot4 {
        .dot;
        animation-delay: 600ms;
    }
}

@keyframes transform {
    0% {
        left: 0;
        opacity: 0;
    }
    5% {
        opacity: 1;
    }
    75% {
        opacity: 1;
    }
    80% {
        left: 100%;
        opacity: 0;
    }
    100% {
        left: 100%;
        opacity: 0;
    }
}
</style>
