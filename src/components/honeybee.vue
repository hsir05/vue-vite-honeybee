<template>
<div class="honeybee">
    <div class="honeybee-body"></div>
    <div class="honeybee-head">
        <div class="honeybee-eye"></div>
        <div class="honeybee-nose"></div>
        <div class="honeybee-mouth"></div>
    </div>
    <div class="wing-left"></div>
    <div class="wing-right"></div>
</div>
</template>
<script setup lang="ts">

</script>
<style lang="scss" scoped>
.honeybee {
    width: 500px;
    height: 500px;
    position: relative;
}

.honeybee-body {
    width: 150px;
    height: 90px;
    position: absolute;
    top: 50%;
    left: 27%;
    transform: translate(-50%, -50%);
    background-color: #ffd400;
    background-image: radial-gradient(circle at 75% 45%, #ffd400 42%, #8a4514 51%, #8a4514 54%, #ffd400 64%, #ffd400 66%, #8a4514 74%, #8a4514 77%, #ffd400 86%);
    border-radius: calc(12 * 1vh) calc(9 * 1vh) calc(9 * 1vh) calc(6 * 1vh);
    z-index: 1;
}

.honeybee-head {
    position: absolute;
    top: 45%;
    left: 28%;
    z-index: 100;
    width: 50px;
    height: 50px;
}

.honeybee-eye {
    position: absolute;

    &::after {
        content: "";
        width: 10px;
        height: 10px;
        border-radius: 50%;
        background-color: #333;
        position: absolute;
        top: 10px;
        left: 5px;
    }

    &::before {
        content: "";
        width: 10px;
        height: 10px;
        border-radius: 50%;
        background-color: #333;
        position: absolute;
        top: 10px;
        left: 50px;
    }
}

.honeybee-mouth {
    position: absolute;
    top: 47%;
    left: 39%;
    width: 20px;
    height: 20px;
    background-color: transparent;
    border: 3px solid #333;
    clip-path: inset(60% 5% 0 5%);
    border-radius: 50%;
    z-index: 2;

}

.wing-left,
.wing-right {
    position: absolute;
    top: 13vh;
    left: calc(9 * 1vh);
    width: calc(8 * 1vh);
    height: calc(16 * 1vh);
    background-color: #48d1cc;
    z-index: 2;
    transform-origin: 75% 100%;
    transform: rotate(-34deg);
    border-radius: calc(8 * 1vh) calc(5 * 1vh) calc(2 * 1vh) calc(10 * 1vh);
    // animation: wing 0.075s infinite alternate ease-in-out;
}

.wing-left {
    left: calc(16 * 1vh);
    z-index: 0;
    transform-origin: 25% 100%;
    transform: rotate(34deg);
    border-radius: calc(5 * 1vh) calc(8 * 1vh) calc(10 * 1vh) calc(2 * 1vh);
}
</style>
