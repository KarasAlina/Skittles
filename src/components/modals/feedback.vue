<template>
  <Modal
    name="feedback"
    size="md"
    title="ЗАДАТЬ ВОПРОС"
    @closeModal="closeModal"
  >
    <template v-slot:content>
      <FeedbackForm></FeedbackForm>
    </template>
  </Modal>
</template>

<script>
import Modal from "@/components/Modal.vue";

import FeedbackForm from "@/components/form/FeedbackForm.vue";

export default {
  components: {
    Modal,
    FeedbackForm,
  },
  data: function () {
    return {};
  },
  methods: {
    closeModal(name) {
      this.$modal.hide(name);
    },

    beforeOpen() {},
  },
};
</script>

<style lang="scss"></style>
