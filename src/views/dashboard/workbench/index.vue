<template>
  <PageWrapper>
    <div class="lg:flex">
      <div class="lg:w-10/10 w-full enter-y">

        <Card>
          <img class="xl:h-50 h-30 mx-auto" src="../../../assets/svg/illustration.svg" />
        </Card>

      </div>
    </div>
  </PageWrapper>
</template>
<script lang="ts" setup>
  import { ref } from 'vue';
  import { Card } from 'ant-design-vue';
  import { PageWrapper } from '/@/components/Page';
  import WorkbenchHeader from './components/WorkbenchHeader.vue';
  import ProjectCard from './components/ProjectCard.vue';
  import QuickNav from './components/QuickNav.vue';
  import DynamicInfo from './components/DynamicInfo.vue';
  import SaleRadar from './components/SaleRadar.vue';

  const loading = ref(true);

  setTimeout(() => {
    loading.value = false;
  }, 1500);
</script>
