<template>
  <div>
    <ul>
      <li v-for="item in items" :key="item.id">
        <slot name="menu-list" :item="item">{{ item }}</slot>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: ["items"]
};
</script>
