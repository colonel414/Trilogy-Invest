<script setup lang="ts">
import { onMounted, ref } from 'vue';
import { Icon } from '@iconify/vue';
import Options from '~/components/utils/options.vue';
import { Menu, MenuItem, MenuItems } from '@headlessui/vue';

const mode = ref<'light' | 'dark'>('light');

const setTheme = (theme: 'light' | 'dark') => {
    mode.value = theme;
    document.documentElement.classList.toggle('dark', theme === 'dark');
};

onMounted(() => {
    const storedTheme = window.localStorage.getItem('theme');
    if (storedTheme && (storedTheme === 'light' || storedTheme === 'dark')) {
        setTheme(storedTheme);
    } else {
        setTheme('light');
    }
});
const toggleTheme = () => {
    setTheme(mode.value === 'dark' ? 'light' : 'dark');
    window.localStorage.setItem('theme', mode.value);
};
// const config = useRuntimeConfig();
</script>

<template>
    <div class="flex items-center pt-5 px-5 mb-3.5">
        <div class="flex items-center">
            <h1 class="text-xl font-bold">Trilogy Investment</h1>
        </div>

        <!-- <Options /> -->
        <div>

            <Menu as="div" class="relative inline-block text-left">
                <transition enter-active-class="transition ease-out duration-100"
                    enter-from-class="transform opacity-0 scale-95" enter-to-class="transform opacity-100 scale-100"
                    leave-active-class="transition ease-in duration-75"
                    leave-from-class="transform opacity-100 scale-100" leave-to-class="transform opacity-0 scale-95">
                    <MenuItems
                        class="absolute right-0 z-10 mt-2 flex space-x-4 origin-top-right bg-white shadow-lg ring-1 ring-black ring-opacity-5 focus:outline-none">
                        <MenuItem v-slot="{ active }">
                        <a href="/" :class="[
                            active ? 'bg-gray-100 text-gray-900' : 'text-gray-700',
                            'block px-4 py-2 text-sm',
                        ]">Home</a>
                        </MenuItem>
                        <MenuItem v-slot="{ active }">
                        <a href="/login" :class="[
                            active ? 'bg-gray-100 text-gray-900' : 'text-gray-700',
                            'block px-4 py-2 text-sm',
                        ]">Login</a>
                        </MenuItem>
                        <MenuItem v-slot="{ active }">
                        <a href="/services" :class="[
                            active ? 'bg-gray-100 text-gray-900' : 'text-gray-700',
                            'block px-4 py-2 text-sm',
                        ]">Services</a>
                        </MenuItem>
                        <MenuItem v-slot="{ active }">
                        <a href="/about-us" :class="[
                            active ? 'bg-gray-100 text-gray-900' : 'text-gray-700',
                            'block px-4 py-2 text-sm',
                        ]">About-Us</a>
                        </MenuItem>
                    </MenuItems>
                </transition>
            </Menu>
        </div>

        <button class="flex h-9 w-9 shrink-0 items-center justify-center rounded-full border bg-background ml-auto"
            @click="toggleTheme">
            <Icon :icon="mode === 'dark' ? 'material-symbols-light:sunny' : 'ri:moon-fill'
                " />
        </button>
    </div>
</template>

<style scoped></style>