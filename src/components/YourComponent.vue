<template>
  <div>
    <h1>商品列表</h1>
    <ul>
      <li v-for="item in items" :key="item.id">
        {{ item.name }} - 数量: {{ item.quantity }} - 价格: {{ item.price }}
      </li>
    </ul>
  </div>
</template>

<script>
import { mockData } from "../warehousemessageemessage";

export default {
  data() {
    return {
      items: mockData
    };
  }
};
</script>
