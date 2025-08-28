<template>
  <el-dialog 
  v-model="centerDialogVisible" 
  :title="props.title" 
  :width="props.width"
   center>
    <span>
      It should be noted that the content will not be aligned in center by
      default
    </span>
    <template #footer>
      <div class="dialog-footer">
        <el-button @click="centerDialogVisible = false">Cancel</el-button>
        <el-button type="primary" @click="centerDialogVisible = false">
          Confirm
        </el-button>
      </div>
    </template>
  </el-dialog>
</template>

<script lang="ts" setup>
import { ref } from 'vue';

const props = withDefaults(defineProps<{
  title?: string;
  width?: number;
}>(), {
  title: 'Warning',
  width: 500
});

const centerDialogVisible = ref(false);

function closeModel() {
    centerDialogVisible.value = false;
}
function openModel() {
    centerDialogVisible.value = true;
}

defineExpose({
    closeModel,
    openModel
});
</script>