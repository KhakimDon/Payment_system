<script setup lang="ts">
import router from '../router'

</script>

<template>
    <div class="w-[100%] h-[100vh] bg-[#F6F9FF] flex items-center justify-center">
        <div class="w-[250px] h-[max-content]">
            <div class="flex items-center justify-center gap-[10px]">
                <img src="https://rf-static.ams3.digitaloceanspaces.com/production/ams3/assets/img/logo.png"
                    alt="RoyalFinance">
                <span class="font-[600] text-[24px]">Payment System</span>
            </div>
            <form @submit.prevent="router.push('/')" class="shadow w-[100%] mt-[30px] rounded-[5px] p-[20px] pt-[30px] bg-white flex flex-col items-center justify-center">
                <span class="font-[400] text-[24px] text-[#012970]">Авторизация</span>
                <div class="flex flex-col mt-[20px] gap-[3px]">
                    <span class="text-[#4A446E]">Имя пользователя:</span>
                    <input class="input h-[40px] border-[1px] border-[#D8DDE1]" type="text">
                </div>
                <div class="flex flex-col mt-[20px] gap-[3px]">
                    <span class="text-[#4A446E]">Пароль:</span>
                    <input class="input h-[40px] border-[1px] border-[#D8DDE1]" type="text">
                </div>
                <div class="flex flex-col mt-[20px] gap-[3px]">
                    <span class="text-[#4A446E]">OTP Token:</span>
                    <input class="input h-[40px] border-[1px] border-[#D8DDE1]" type="text">
                </div>
                <button class="btn bg-[#0D6EFD] w-[100%] text-white hover:bg-[#2968c7] mt-[30px]">Вход</button>
            </form>
        </div>
    </div>
</template>

<style>
.shadow{
    box-shadow: 0 0 30px #eaeffc;
}
</style>
