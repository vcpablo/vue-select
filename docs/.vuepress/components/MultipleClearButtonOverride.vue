<template>
  <div>
    <v-select
            multiple
            v-model="selected"
            :options="['Canada', 'United States']"
            :components="{Deselect}"
    />
  </div>
</template>

<script>
export default {
  data: () => ({
    selected: ['Canada'],
    Deselect: {
      render: createElement => createElement('span', '❌'),
    },
  }),
};
</script>
