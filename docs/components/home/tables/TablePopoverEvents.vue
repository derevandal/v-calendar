<template>
<b-table
  :data='props'>
  <template scope='props'>
    <b-table-column label='Name'>
      <span v-html='props.row.name'></span>
    </b-table-column>
    <b-table-column label='Description'>
      <span v-html='props.row.description'></span>
    </b-table-column>
    <b-table-column label='Parameters'>
      <span v-html='props.row.parameters'></span>
    </b-table-column>
  </template>
</b-table>
</template>

<script>
export default {
  data() {
    const props = [
      {
        name: '<code>willAppear</code>',
        description: 'Content popover is about to appear.',
      },
      {
        name: '<code>didAppear</code>',
        description: 'Content popover is about to appear.',
      },
      {
        name: '<code>willDisappear</code>',
        description: 'Content popover is about to disappear.',
      },
      {
        name: '<code>didDisappear</code>',
        description: 'Content popover is about to disappear.',
      },

    ];
    return {
      props,
    };
  },
};
</script>
