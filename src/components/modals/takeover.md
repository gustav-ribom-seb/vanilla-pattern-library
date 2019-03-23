---
title: Takeover
componentid: component-takeover
variantid: normal
guid: component-takeover-normal
---

# Usage

Import classes:

```scss
@import "~@sebgroup/vanilla/src/components/modals/takeover";
```

Use them in your template:

```html
<div class="sdv-takeover">...</div>
```

To activate the modal, add the `-sdv-modal-active` modifier:

```html
<div class="sdv-takeover -sdv-modal-active">
  ...
</div>
```

---

You can also use the mixins:

```scss
@import "~@sebgroup/vanilla/src/components/modals/takeover-mixins";
@import "~@sebgroup/vanilla/src/components/modals/modal-mixins";

.my-modal-class {
  @include vanilla-takeover();
}
```

:::componentpreview


## Normal

```html
<div class="sdv-takeover -sdv-modal-active">
  <div class="sdv-takeover__container">
    <header class="sdv-takeover__header">
      <h3 class="sdv-takeover__heading">Modal Heading</h3>
      <button class="sdv-takeover__close">
        <i class="fal fa-times"></i>
      </button>
    </header>
    <div class="sdv-takeover__content">
      <h4>Modal Content</h4>
      <p>Lorem ipsum dolor sit amet</p>
    </div>
  </div>
  <div class="sdv-modal-backdrop sdv-modal-backdrop--fold-in"></div>
</div>
```
## Interactive

```html
<div class="sdv-takeover" id="takeover">
    <div class="sdv-takeover__container">
        <header class="sdv-takeover__header">
            <h3 class="sdv-takeover__heading">Modal Heading</h3>
      <button class="sdv-takeover__close">
          <a href="#">
              <i class="fal fa-times"></i>
        </a>
      </button>
    </header>
    <div class="sdv-takeover__content">
        <h4>Modal Content</h4>
      <p>Lorem ipsum dolor sit amet</p>
    </div>
  </div>
  <div class="sdv-modal-backdrop sdv-modal-backdrop--fold-in"></div>
</div>
<a href="#takeover" style="align-self: flex-end;">Open takeover</a>
<span id="#"></span>
```

:::
