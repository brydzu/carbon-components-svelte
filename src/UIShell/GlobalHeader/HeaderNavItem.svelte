<script>
  /**
   * Specify the `href` attribute
   * @type {string} [href]
   */
  export let href = undefined;

  /**
   * Specify the text
   * @type {string} [text]
   */
  export let text = undefined;

  /**
   * Obtain a reference to the HTML anchor element
   * @type {null | HTMLAnchorElement} [ref=null]
   */
  export let ref = null;
</script>

<li>
  <a
    bind:this="{ref}"
    role="menuitem"
    tabindex="0"
    href="{href}"
    class:bx--header__menu-item="{true}"
    {...$$restProps}
    on:click
    on:mouseover
    on:mouseenter
    on:mouseleave
    on:keyup
    on:keydown
    on:focus
    on:blur
  >
    <span class:bx--text-truncate--end="{true}">{text}</span>
  </a>
</li>
