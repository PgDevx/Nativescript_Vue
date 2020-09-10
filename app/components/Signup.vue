<template>
    <Page class="page">
        <ActionBar class="action-bar">
            <Label text="My App" class="title">
        </ActionBar>
        <FlexboxLayout class="main-signup">
            <StackLayout class="form">
                <StackLayout class="input-field">
                    <TextField v-model="Username" hint="Username"
                        class="test" />
                </StackLayout>
                <StackLayout class="input-field">
                    <TextField v-model="Password" hint="Password"
                        class="test" />
                </StackLayout>
                <StackLayout class="input-field">
                    <TextField v-model="Password" hint="Confirm-Password"
                        class="test" />
                </StackLayout>
                <Button text="SignUp" @tap="Login" class="btn-sig" />
            </StackLayout>
        </FlexboxLayout>
    </Page>
</template>

<script>
    import Login from "./Login";
    export default {
        methods: {
            Login() {
                this.$navigateTo(Login);
            }
        }
    };
</script>

<style scoped>
</style>