<template>
    <div class="flex h-screen w-full items-center justify-center bg-gray-900 bg-cover bg-no-repeat"
        style="background-image:url('https://images.unsplash.com/photo-1605184861755-8f190fea96a5?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1966&q=80')">
        <div class="rounded-xl bg-white bg-opacity-10 px-16 py-10 shadow-lg backdrop-blur-md max-sm:px-8">
            <div class="text-white">
                <form action="#">
                    <div class="mb-4 text-lg">
                        <input
                            class="rounded-xl border-none bg-white-400 bg-opacity-50 px-6 py-2 text-center text-inherit placeholder-slate-200 shadow-lg outline-none backdrop-blur-md"
                            type="text" name="name" placeholder="id@email.com" />
                    </div>

                    <div class="mb-4 text-lg">
                        <input
                            class="rounded-xl border-none bg-white-400 bg-opacity-50 px-6 py-2 text-center text-inherit placeholder-slate-200 shadow-lg outline-none backdrop-blur-md"
                            type="Password" name="name" placeholder="*********" />
                    </div>
                    <div class="mt-8 flex justify-center text-lg text-black">
                        <button type="submit"
                            class="rounded-xl bg-white-400 bg-opacity-50 px-10 py-2 text-white shadow-xl backdrop-blur-md transition-colors duration-300 hover:bg-pink-600">Login</button>
                    </div>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            username: '',
            password: '',
        }
    },
    methods: {
        register() {
            console.log(`Username: ${this.username}, Password: ${this.password}`);
            // handle registration logic here
        },
    },
}
</script>
  