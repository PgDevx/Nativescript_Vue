<template>
    <Page class="page">
        <ActionBar class="action-bar">
            <Label text="My App" class="title">
        </ActionBar>
        <FlexboxLayout class="main-login">
            <StackLayout class="form">
                <StackLayout class="input-field">
                    <TextField v-model="Username" hint="Username"
                        class="test" />
                </StackLayout>
                <StackLayout class="input-field">
                    <TextField v-model="Password" hint="Password"
                        class="test" />
                </StackLayout>

                <Button text="Log in" @tap="submit()" class="btn-log" />
            </StackLayout>
        </FlexboxLayout>
    </Page>
</template>

<script>
    export default {
        data() {
            return {
                textFieldValue: ""
            };
        },
        methods: {
            submit() {
                alert("Login Successful");
            }
        }
    };
</script>

<style scoped>

</style>