# Changelog

### v3.0.0

- Typescript support

### v2.3.0

- Stops using autobind-decorator.
- Adds `<input type="submit" />` to forms to enable submitting on enter.

### v2.2.0

- Clones the state prop.
- Check state changes using deep equal comparison.
- Props not specified in propTypes are passed to fields too.

### v2.1.0 (Mayor rewrite)

- Upgrade to React 16.
- Use the new Context API.
- New `WithValue` HOC.
- Better testing (without enzyme).
- Almost 100% backwards compatible.
- Field input ref is now in `.input` instead of `.refs.input`.

### v2.0.1

- Add focus method to Field.

### v2.0.0

- Complete rewrite.
- Faster and lighter.
- Better state management.
- `doc` prop is deprecated.
- No more simple-schema integration.
- No more collection integration.
- No more Meteor integration

### v1.9.0

- Allow autogenerated forms from schemas that contain arrays with primitive values. by @prinzdezibel at [#59](https://github.com/nicolaslopezj/simple-react-form/pull/59).

### v1.8.1

- submit function returns a boolean indicating the result.

### v1.8.0

- Use lodash instead of underscore.
- Use deepClone instead of clone to clone doc, state, and errorMessages props.

### v1.7.9

- Not render form never in React Native
- Add `errorMessages` prop to `Form`
- Pass props not present in propTypes to form element

### v1.7.7

- Fix onSubmit doc cleaning

### v1.7.6

- Fix use of this.props on Form constructor

### v1.7.4

- Pass only present fields in `onSubmit` callback.

### v1.7.3

- Set field type prop label to any to avoid warnings.

### v1.7.2

- Fix a bug with `unregisterField`.

### v1.7.1

- Separate `generateInputsForKeys` from `Form.js`.
- Fix a bug with `getPresentFields` with deep keys.
- Add tests for `generateInputsForKeys` and `getPresentFields`.

### v1.7.0

- Tests. by @fermuch at [#36](https://github.com/nicolaslopezj/simple-react-form/pull/36).
- Check javascript style when testing (js-standard).
- Is no longer required to extend the FieldType to create fields.
- Rename files.
- Better warning when field has no field type.
- Check React Native in other way.

### v1.6.15

- Fix bug created by using dot-object as a dependency instead of including the code.

### v1.6.14

- Use dot-object as a dependency instead of including the code.
- Create tests for clean fields function.
- Put utility functions into different files.

### v1.6.13

- Set the prop clearOnSuccess default to false.

### v1.6.12

- Clears the form (insert and function types) when onSuccess is called. By [@fermuch](https://github.com/fermuch) at [#28](https://github.com/nicolaslopezj/simple-react-form/pull/28).

### v1.6.11

- Nulls are also filtered when updating.

### v1.6.10

- Set changes to blank before passing the onSuccess callback. Fixes [#4](https://github.com/nicolaslopezj/simple-react-form/issues/4).

### v1.6.9

- Better error handling when getting errors from the server.

### v1.6.8

- Improve the algorithm that was implemented in 1.6.6. This fixes when fields that
  are object are removed from the update object.

### v1.6.6

- Disabled fields don't count as registered fields when passing to modifiers.

### v1.6.5

- `keepArrays` is now `true` by default.
- `commitOnlyChanges` is now `false` by default.
- When updating a document, only fields that are present in the form (registered
  in the main form component) will be passed to the modifiers.

### v1.6.4

- Accept any type of label in field.

### v1.6.3

- Fix a bug with object or array fields in nested array with simple schema.

### v1.6.1

- `keepArrays` prop is now default `false`.

### v1.6

- Array and object components are fields now.

### v1.5

- Field types should be passed in the type prop of the Field component.

### v1.4.1

- Support for React Native.
- Add useFormTag option.

### v1.4

- Use context instead of cloning elements.
