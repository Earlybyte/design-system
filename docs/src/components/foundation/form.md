# Form

The indispensable form controls, designed for maximum clarity.
Form elements are used in combination with the CSS grid system.

## Form fields

A basic form field has his container element `bal-field` and 3 child elements:

- `bal-field-label` for adding a label to the form control.
- `bal-field-control` to contain the control like an input.
- `bal-field-message` to show validation message or helper messages.

<docs-demo>
  <form class="columns is-multiline mt-0 has-background-white">
    <bal-field class="column is-full py-0" expanded>
      <bal-field-label>Firstname</bal-field-label>
      <bal-field-control>
        <bal-input placeholder="Enter your firstname"></bal-input>
      </bal-field-control>
      <bal-field-message color="danger">Required Field</bal-field-message>
    </bal-field>
  </form>
</docs-demo>

```html
<bal-field expanded>
  <bal-field-label>Firstname</bal-field-label>
  <bal-field-control>
    <bal-input placeholder="Enter your firstname"></bal-input>
  </bal-field-control>
  <bal-field-message color="danger">Required Field</bal-field-message>
</bal-field>
```

## Combine fields

With the help of our [CSS Grid](/components/foundation/grid.html) we can assemble the form fields to nice looking form.

- First we add the container element `<form class="columns is-multiline mt-0">`
  - `is-multiline` enables us to have multiple rows in our form grid
  - `mt-0` resets the margin top to 0px
- Each field is used as a column `<bal-field class="column is-full py-0" expanded>`
  - `is-full` takes the full width
  - `py-0` removes the padding on top and bottom

<docs-demo>
  <form class="columns is-multiline mt-0 has-background-white">
    <bal-field class="column is-full py-0" expanded>
      <bal-field-control>
        <bal-radio-group>
          <bal-radio name="gender" value="male">Male</bal-radio>
          <bal-radio name="gender" value="female">Female</bal-radio>
        </bal-radio-group>      
      </bal-field-control>
    </bal-field>
    <bal-field class="column is-half py-0" expanded>
      <bal-field-label>Firstname</bal-field-label>
      <bal-field-control>
        <bal-input placeholder="Enter your firstname"></bal-input>
      </bal-field-control>
    </bal-field>
       <bal-field class="column is-half py-0" expanded>
      <bal-field-label>Lastname</bal-field-label>
      <bal-field-control>
        <bal-input placeholder="Enter your lastname"></bal-input>
      </bal-field-control>
    </bal-field>
  </form>
</docs-demo>

```html{1,2,10,16}
<form class="columns is-multiline mt-0">
  <bal-field class="column is-full py-0" expanded>
    <bal-field-control>
      <bal-radio-group>
        <bal-radio name="gender" value="male">Male</bal-radio>
        <bal-radio name="gender" value="female">Female</bal-radio>
      </bal-radio-group>
    </bal-field-control>
  </bal-field>
  <bal-field class="column is-half py-0" expanded>
    <bal-field-label>Firstname</bal-field-label>
    <bal-field-control>
      <bal-input placeholder="Enter your firstname"></bal-input>
    </bal-field-control>
  </bal-field>
  <bal-field class="column is-half py-0" expanded>
    <bal-field-label>Lastname</bal-field-label>
    <bal-field-control>
      <bal-input placeholder="Enter your lastname"></bal-input>
    </bal-field-control>
  </bal-field>
</form>
```

### More examples

- [Form Template with a contact form](/components/templates/contact-form.html)
