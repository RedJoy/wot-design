<template>
  <label
    class="wd-radio"
    :class="{
      'is-checked': isChecked,
      'is-button': finalShape === 'button',
      'is-disabled': finalDisabled,
      'is-inline': inline
    }"
  >
    <div
      class="wd-radio__label"
      :style="[{ 'color': isChecked && finalShape === 'button' && !finalDisabled ? finalCheckedColor : '' }, {'max-width': maxWidth}]"
    >
      <slot></slot>
    </div>
    <span
      class="wd-radio__shape"
      :style="{ 'color': isChecked && !finalDisabled ? finalCheckedColor : '' }"
    >
      <i
        class="wd-icon-check"
        :style="{
          'color': isChecked && !finalDisabled ? finalCheckedColor : ''
        }"
      ></i>
      <input
        type="radio"
        class="wd-radio__input"
        :value="value"
        :checked="isChecked"
        :disabled="finalDisabled"
        @change="handleChange"
      />
    </span>
  </label>
</template>

<script>
export default {
  name: 'WdRadio',
  inject: ['radioGroup'],
  props: {
    value: [String, Number, Boolean],
    shape: String,
    checkedColor: String,
    maxWidth: String,
    disabled: Boolean
  },
  computed: {
    isChecked () {
      return this.radioGroup.value === this.value
    },
    finalShape () {
      return this.shape || this.radioGroup.shape
    },
    finalCheckedColor () {
      return this.checkedColor || this.radioGroup.checkedColor
    },
    finalDisabled () {
      return this.disabled || this.radioGroup.disabled
    },
    inline () {
      return this.radioGroup.inline
    }
  },
  methods: {
    handleChange () {
      this.radioGroup.changeValue(this.value)
    }
  }
}
</script>
