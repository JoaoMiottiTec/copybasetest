<script setup>
/* const axios = require("axios").default;

const axios = require('axios'); */
</script>

<template>
  <form action="/import-excel" enctype="multipart/form-data" method="post">
    <div class="field">
      <div class="file is-boxed is-primary">
        <label class="file-label">
          <input
            type="file"
            ref="file"
            name="import-excel"
            @change="selectFile"
            class="file-input"
            accept="application/vnd.openxmlformats-officedocument.spreadsheetml.sheet, application/vnd.ms-excel"
          />

          <span class="file-cta">
            <span class="file-icon">
              <i class="fas fa-upload"></i>
            </span>
            <span class="file-label"> Escolha um arquivo </span>
          </span>

          <span v-if="file" class="file-name">{{ file.name }}</span>
        </label>
      </div>
    </div>
    <button type="submit" value="Store File"></button>
  </form>
</template>

<style></style>
