<script>
export default {
  name: 'DataTable',
  props: {
    headers: {
      type: Array,
      required: true, // 필수
    },
    items: {
        type: Array,
        default: () => [],
    }
  },
  computed: {
    headerKey() {
        return this.headers.map((header) => header.value);
    }
  }
};
</script>

<template>
    <div class="data_table">
      <table>
        <thead>
          <tr>
            <!-- 컬럼명 바인딩 -->
            <th v-for="header in headers" :key="header.text">
              {{ header.text }}
            </th>
          </tr>
        </thead>
        <tbody>
            <!-- TODO 테이블 데이터 바인딩 -->
            <tr v-for="(item, index) in items" :key="index">
                <td v-for="key in headerKey" :key="key + index">
                    {{ item[key] }}
                </td>
            </tr>
        </tbody>
      </table>
    </div>
</template>