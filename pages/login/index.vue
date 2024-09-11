<template>
    <div class="min-h-screen flex items-center justify-center bg-gray-100">
        <div class="bg-white p-8 rounded-lg shadow-lg w-full max-w-sm">
            <h2 class="text-2xl font-bold text-center mb-6">Login</h2>
            <form @submit.prevent="handleLogin">
                <div class="mb-4">
                    <label for="email" class="block text-gray-700 font-bold mb-2">Email</label>
                    <input v-model="email" type="email" id="email"
                        class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:border-blue-500" required />
                </div>
                <div class="mb-6">
                    <label for="password" class="block text-gray-700 font-bold mb-2">Password</label>
                    <input v-model="password" type="password" id="password"
                        class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:border-blue-500" required />
                </div>
                <button type="submit"
                    class="w-full bg-blue-500 text-white py-2 rounded-lg hover:bg-blue-600 transition duration-300">
                    Login
                </button>
            </form>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'

const email = ref('')
const password = ref('')

const handleLogin = () => {
    console.log('Logging in with', email.value, password.value)
}
</script>