<template>
    <div class="min-h-screen bg-gray-100 py-16">
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
    </div>
</template>

<script lang="ts">
export default {
    name: "ServicesPage",
};
</script>

<style scoped></style>