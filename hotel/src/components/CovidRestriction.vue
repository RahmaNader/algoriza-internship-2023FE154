<template>
    <div class="danger">
        <img class="danger-icon" src="../assets/danger1.png" alt="Danger Icon" />
        <p class="danger-text">Check the latest COVID-19 restrictions before you travel. Learn more</p>
    </div>
</template>

<script>
export default {
    name: 'CovidRestriction',
    // Your script code here
}
</script>

<style scoped>
.danger {
  position: absolute;
  width: 90%;
  height: 72px;
  left: 100px;
  top: 662px;
  background: #FCEFCA;
  border-radius: 8px;
    display: flex;
    align-items: center;
}

.danger-icon {
  width: 20px;
  height: 20px;
  flex: none;
  order: 0;
  margin: 0 20px;
}

</style>
