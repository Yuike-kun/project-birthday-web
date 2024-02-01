<script setup>
import 'bootstrap-icons/font/bootstrap-icons.css'
import Input from './Input.vue'
</script>

<template>
    <section id="join" class="bg-gradient-to-r from-indigo-500 to-green-500 w-full text-slate-100">
        <div class="grid grid-cols-1 lg:grid-cols-3 place-content-center items-center">
            <div class="lg:border-e-2 border-b-2 lg:border-b-0 text-center p-4">
                <span class="font-bold text-6xl">
                    WANT TO JOIN US?
                </span>
            </div>
            <div class="col-span-2 p-3">
                <span class="text-2xl capitalize">
                    To Join us, you can simply contact us :3
                </span>
                <div class="text-lg grid-cols-4 grid w-48">
                    <div class="col-span-1">
                        <i class="bi bi-whatsapp"></i>
                    </div>
                    <span class="col-span-3">
                        0154165151156145
                    </span>
                    <div class="col-span-1">
                        <i class="bi bi-instagram"></i>
                    </div>
                    <span class="col-span-3">
                        @yuikekun_
                    </span>
                    <div class="col-span-1">
                        <i class="bi bi-telephone"></i>
                    </div>
                    <span class="col-span-3">
                        121-117-105
                    </span>
                </div>
            </div>
        </div>
    </section>

    <div class="border-2 w-1/2 rounded border-slate-50"></div>

    <fieldset
        class="bg-neutral-900 px-4 py-10 w-[75vw] rounded text-neutral-100 flex flex-col shadow-lg shadow-neutral-800">
        <span class="text-3xl font-bold text-center"> Give us your opinion </span>
        <small class="text-center"> Note : This is a dummy </small>

        <div class="flex flex-col gap-5 items-center">
            <div class="grid grid-cols-1 w-11/12">
                <Input type="text" label="Your Name" name="name"/>
            </div>
            <div class="grid grid-cols-1 w-11/12">
                <Input type="text" label="Your Opinion" name="kesan"/>
            </div>
            <div class="grid grid-cols-1 w-11/12">
                <Input type="text" label="Is There Anything more?" name="pesan"/>
            </div>
            <button
                class="border w-11/12 py-2 rounded-md hover:bg-slate-100 hover:text-neutral-900 transition-all duration-300">
                Send Your Opinion
            </button>
        </div>
    </fieldset>
</template>