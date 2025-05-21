<template>
  <div class="flex items-center justify-center min-h-screen bg-amber-500">
    <div
      class="relative flex flex-col m-6 space-y-8 bg-white shadow-2xl rounded-2xl md:flex-row md:space-y-0 md:space-x-6"
    >
      <!-- Lado derecho -->
      <div class="flex flex-col justify-center p-8 md:p-14 w-full md:w-[400px]">
        <span class="text-center mb-3 text-4xl font-bold tracking-wider">
          LOGO
        </span>
        <span class="text-center font-light text-gray-400 mb-8">
          Panel Administrativo
        </span>

        <!-- Campo Email -->
        <div class="py-2">
          <label for="email" class="mb-2 text-md block">Email</label>
          <input
            type="email"
            id="email"
            name="email"
            required
            autocomplete="email"
            autofocus
            class="w-full p-2 border border-gray-300 rounded-md placeholder:font-light placeholder:text-gray-500"
            placeholder="ejemplo@correo.com"
          />
        </div>

        <!-- Campo Password -->
        <div class="py-2">
          <label for="pass" class="mb-2 text-md block">Password</label>
          <input
            type="password"
            id="pass"
            name="pass"
            required
            autocomplete="current-password"
            class="w-full p-2 border border-gray-300 rounded-md placeholder:font-light placeholder:text-gray-500"
            placeholder="••••••••"
          />
        </div>

        <!-- Botón -->
        <div class="flex flex-col items-center pt-6">
          <button
            type="submit"
            class="w-full box-border border border-transparent bg-black text-white p-2 rounded-lg transition-all duration-300 hover:cursor-pointer hover:bg-amber-500 hover:text-white hover:border-gray-300"
          >
            Ingresar
          </button>
        </div>
      </div>
    </div>
  </div>
</template>


<script setup>

</script>

<style lang="scss" scoped>

</style>