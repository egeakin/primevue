<template>
    <div class="p-card p-component ui-card-shadow" style="width: 360px;">
        <div class="p-card-header" v-if="$slots.header">
            <slot name="header"></slot>
        </div>
        <div class="p-card-body">
            <div class="p-card-title" v-if="$slots.title"><slot name="title"></slot></div>
            <div class="p-card-subtitle" v-if="$slots.subtitle"><slot name="subtitle"></slot></div>
            <div class="p-card-content">
                <slot name="content"></slot>
            </div>
            <div class="p-card-footer" v-if="$slots.footer">
                <slot name="footer"></slot>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.p-card-header img {
    width: 100%;
}

.p-card-body {
    padding: 1em;
}

.p-card-title {
    font-size: 1.5em;
    font-weight: bold;
    margin-bottom: .5em;
}

.p-card-subtitle {  
    opacity: .7;
    margin-bottom: .5em;
    margin-top: -.25em;
    font-weight: bold;
}

.p-card-footer {
    padding-top: 1em;
}
</style>