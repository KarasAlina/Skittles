<template>
  <Modal
    name="success_feedback"
    :success="true"
    title="Спасибо!"
    @closeModal="closeModal"
  >
    <template v-slot:content>
      <div class="success_modal">
        <p class="modal__text success_modal__text">
          Спасибо за обращение! Мы скоро Вам ответим!
        </p>
        <div class="success_modal__footer"></div>
      </div>
    </template>
  </Modal>
</template>

<script>
import Modal from "@/components/Modal.vue";

export default {
  components: {
    Modal,
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
