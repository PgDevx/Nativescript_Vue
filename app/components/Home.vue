<template>
    <Page class="page">
        <ActionBar class="action-bar">
            <Label text="My App" class="title">
        </ActionBar>
        <FlexboxLayout class="main">
            <StackLayout>
                <StackLayout class="image">
                    <Image src="~/images/NS-Vue-Logo.png" stretch="none"
                        class="img" />
                    <Label textWrap="true" text="Welcome to My App!"
                        class="lable" />
                </StackLayout>
                <FlexboxLayout class="inside">
                    <FlexboxLayout>
                        <Button text="Log in" @tap="Login" class="btn" />
                    </FlexboxLayout>
                    <FlexboxLayout>
                        <Button text="Sign Up" @tap="SignUp()" class="btn" />
                    </FlexboxLayout>
                </FlexboxLayout>
            </StackLayout>
        </FlexboxLayout>
    </Page>
</template>

<script>
    import Login from "./Login";
    import Signup from "./Signup";
    export default {
        data() {
            return {};
        },
        methods: {
            Login() {
                this.$navigateTo(Login);
            },
            SignUp() {
                this.$navigateTo(Signup);
            }
        }
    };
</script>

<style scoped>

</style>