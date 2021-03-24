<template>
  <div class="experience">
    <NavBreadcrumb :trail="['Home', 'Experience']" />
    <h1>This is an experience page</h1>
  </div>
</template>

<script>
import NavBreadcrumb from "@/components/NavBreadcrumb";

export default {
  name: "Experience",
  components: {
    NavBreadcrumb
  }
};
</script>