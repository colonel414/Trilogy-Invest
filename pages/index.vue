<template>
    <div class="min-h-screen bg-gray-50">
        <!-- Navbar -->
        <Navbar />

        <!-- Hero Section -->
        <section class="bg-blue-800 text-white relative pt-32 pb-16">
            <div class="absolute inset-0 bg-cover bg-center"
                style="background-image: url('https://images.unsplash.com/photo-1554232024-93866ba096a3?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxmZWF0dXJlZC1waG90b3MtZmVlZHw0OHx8fGVufDB8fHx8fA%3D%3D=rb-1.2.1&q=80&w=1080');">
            </div>
            <div class="relative container mx-auto px-6 text-center">
                <h2 class="text-5xl font-bold leading-tight mb-6">Transforming Businesses with Expertise</h2>
                <p class="text-lg mb-8">
                    Trilogy Consulting specializes in Logistics, Water Engineering, and IT Solutions. Discover how our
                    tailored solutions can drive your success.
                </p>
                <a href="#services"
                    class="bg-white text-blue-800 font-semibold py-3 px-6 rounded-full shadow-lg hover:bg-gray-200 transition duration-300">
                    Explore Our Services
                </a>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="py-16">
            <div class="container mx-auto px-6">
                <div class="text-center">
                    <h3 class="text-4xl font-semibold text-gray-900 mb-6">About Trilogy Consulting</h3>
                    <p class="text-lg text-gray-700 max-w-4xl mx-auto">
                        Trilogy Consulting offers expert services in Logistics, Water Engineering, and IT Solutions. We
                        leverage our deep industry knowledge to deliver innovative, effective solutions tailored to your
                        unique business needs. Our approach combines strategic insight with practical implementation,
                        ensuring measurable results and sustainable growth.
                    </p>
                </div>
            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="bg-gray-100 py-16">
            <div class="container mx-auto px-6 text-center">
                <h3 class="text-4xl font-semibold text-gray-900 mb-8">Our Services</h3>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-12">
                    <!-- Service 1 -->
                    <div class="bg-white shadow-lg p-8 rounded-lg">
                        <img src="https://images.unsplash.com/photo-1473445730015-841f29a9490b?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTl8fGxvZ2lzdGljc3xlbnwwfHwwfHx8MA%3D%3D=rb-1.2.1&q=80&w=1080"
                            alt="Logistics Consulting" class="w-full h-48 object-cover rounded-lg mb-4" />
                        <h4 class="text-2xl font-bold text-gray-900 mb-4">Logistics Consulting</h4>
                        <p class="text-gray-700">
                            Enhance your supply chain management with our expert logistics consulting services, designed
                            to optimize efficiency and reduce costs.
                        </p>
                    </div>
                    <!-- Service 2 -->
                    <div class="bg-white shadow-lg p-8 rounded-lg">
                        <img src="https://plus.unsplash.com/premium_photo-1667520087776-ed55ab3ec406?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MXx8d2F0ZXIlMjBlbmdpbmVlcnxlbnwwfHwwfHx8MA%3D%3D=rb-1.2.1&q=80&w=1080"
                            alt="Water Engineering" class="w-full h-48 object-cover rounded-lg mb-4" />
                        <h4 class="text-2xl font-bold text-gray-900 mb-4">Water Engineering Solutions</h4>
                        <p class="text-gray-700">
                            We provide sustainable water management solutions tailored to your needs, ensuring effective
                            and environmentally friendly outcomes.
                        </p>
                    </div>
                    <!-- Service 3 -->
                    <div class="bg-white shadow-lg p-8 rounded-lg">
                        <img src="https://images.unsplash.com/photo-1720048170970-3848514c3d60?w=500&auto=format&fit=crop&q=60&ixlib=rb-4.0.3&ixid=M3wxMjA3fDF8MHxmZWF0dXJlZC1waG90b3MtZmVlZHwxfHx8ZW58MHx8fHx8=rb-1.2.1&q=80&w=1080"
                            alt="IT Consulting" class="w-full h-48 object-cover rounded-lg mb-4" />
                        <h4 class="text-2xl font-bold text-gray-900 mb-4">IT Consulting & Solutions</h4>
                        <p class="text-gray-700">
                            Our IT consulting services offer innovative solutions to help your business stay ahead in
                            the digital landscape, driving growth and transformation.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="py-16 bg-blue-800 text-white">
            <div class="container mx-auto px-6 text-center">
                <h3 class="text-4xl font-semibold mb-8">Get in Touch</h3>
                <p class="text-lg mb-8">We would love to hear from you. Reach out to discuss how Trilogy Consulting can
                    support your business goals.</p>
                <a href="mailto:info@trilogyconsulting.com"
                    class="bg-white text-blue-800 font-semibold py-3 px-6 rounded-full shadow-lg hover:bg-gray-200 transition duration-300">
                    Contact Us
                </a>
            </div>
        </section>

        <!-- Footer -->
        <footer class="bg-gray-800 text-white py-4">
            <div class="container mx-auto px-6 text-center">
                <p>&copy; 2024 Trilogy Consulting. All rights reserved.</p>
            </div>
        </footer>
    </div>
</template>

<script lang="ts">
import Navbar from '~/components/utils/navbar.vue';

export default {
    components: {
        Navbar,
    },
};
</script>