<script>
export default {
  name: 'FdActionBarTitle',
  props: {
    // Name of a tag that will be used to wrap the title/default slot.
    tag: {
      type: String,
      // `h3` – by default the title will be wrapped inside an `h3`-element.
      default: 'h3'
    }
  },
  render(h) {
    const data = { class: 'fd-action-bar__title' }
    return h(this.tag, data, this.$slots.default)
  }
}
</script>
