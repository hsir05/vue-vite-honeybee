<template>
<div class="honeybee">
    <div class="honeybee-body"></div>
</div>
</template>
<script setup lang="ts">

</script>
<style lang="scss" scoped>
.honeybee{

}
.honeybee-body{
    width: 150px;
    height: 90px;
    background-color: #ffd400;
    background-image: radial-gradient(circle at 75% 45%, #ffd400 42%, #8a4514 51%, #8a4514 54%, #ffd400 64%, #ffd400 66%, #8a4514 74%, #8a4514 77%, #ffd400 86%);
    border-radius: calc(12 * 1vh) calc(9 * 1vh) calc(9 * 1vh) calc(6 * 1vh);
    z-index: 1;
}
</style>
