<template>
  <div>
    <label :for="identity" class="fw-semibold">{{ label }} <span style="color: #cb3a31">*</span></label>
    <textarea
      class="form-control"
      :id="identity"
      :placeholder="placeholder"
    ></textarea>
  </div>
</template>

<script setup>
defineProps({
  identity: { type: String, require: true },
  label: { type: String, require: true },
  placeholder: { type: String, require: true },
});
</script>