<template>
    <div>
        <slot name="icon"></slot>
    </div>
</template>

<style scoped>
    div {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 50px;
        width: 50px;
        color: var(--vt-c-text-dark-2);
        border: 1px solid var(--vt-c-divider-dark-2);
        border-radius: 8px;
        margin: 15px;
    }
    div:before {
        content: "";
        border-bottom: 1px solid #ffffff;
        width: 15px;
        position: absolute;
        left: -16px;
    }
    div:after {
        content: "";
        border-bottom: 1px solid #ffffff;
        width: 15px;
        position: absolute;
        right: -16px;
    }
</style>