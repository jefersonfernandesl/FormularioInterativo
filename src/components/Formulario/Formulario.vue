<script setup>
import Input from './Input.vue'
</script>

<template>
    <form action="" class="flex p-4 gap-10">
        <Input label-text="Nome" input-id="product_name" type="text" name="product_name" id="product_name" placeholder="Digite o nome do produto" />
        <Input label-text="Quantidade" input-id="product_quantity"  type="number" name="product_quantity" id="product_quantity" placeholder="Digite a quantidade do produto" />
    </form>
</template>