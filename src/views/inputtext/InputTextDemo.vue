<template>
    <div>
        <div class="content-section introduction">
            <div class="feature-intro">
                <h1>InputText</h1>
                <p>InputText renders and input field where the user can enter data.</p>
            </div>
        </div>

        <div class="content-section implementation">
            <h3 class="first">Basic</h3>
            <InputText type="text" v-model="value1" />
            <span :style="{marginLeft: '.5em'}">{{value1}}</span>

            <h3>Floating Label</h3>
            <span class="p-float-label">
                <InputText id="username" type="text" v-model="value2" />
                <label for="username">Username</label>
            </span>

            <h3>Disabled</h3>
            <InputText type="text" v-model="value3" disabled />
        </div>

        <InplaceTextDoc />
    </div>
</template>

<script>
import InputTextDoc from './InputTextDoc';

export default {
    data() {
        return {
            value1: '',
            value2: '',
            value3: 'PrimeVue'
        }
    },
	components: {
		'InputTextDoc': InputTextDoc
	}
}
</script>

<style>

</style>
