# Guide: Action editor

### Overview <a href="#h_9f94ea4deb" id="h_9f94ea4deb"></a>

The Action Editor allows you to define a sequence of actions (based on Test Case steps) to be performed during automated testing. Each action has a `type`, a `text` step description, and may require a `selector` and/or a `value`, depending on the action type. Actions are structured as an array of objects.

### Action Structure <a href="#h_178334086a" id="h_178334086a"></a>

Each action is a JSON object with the following properties:

* `type`: (string, required and non-empty) Specifies the type of action to be performed.
* `text`: (string, required and non-empty) A human-readable description of the step.
* `selector`: (string, conditionally required and non-empty) A CSS selector that identifies the target element for the action. Required for actions that interact with specific elements on the page.
* `value`: (string, conditionally required and non-empty) A value associated with the action. Required for actions that involve providing input or making assertions about specific values.
* `automated`: (boolean, readonly) Indicated whether the step associated with the action has been already successfully automated or not.
* `reason`: (string, readonly) A description of the error the action returned.

### Action Types and Descriptions <a href="#h_c8f18c0c7c" id="h_c8f18c0c7c"></a>

The following action types are supported:

* `goto`: Navigates the browser to a specified URL. Requires a `value` representing the URL.
* `click`: Clicks on an element identified by a CSS selector. Requires a `selector` to specify the element to click.
* `fill`: Fills a form field (identified by a CSS selector) with a specified value. Requires a `selector` to identify the field and a `value` to fill it with.
* `check`: Checks a checkbox (identified by a CSS selector). Requires a `selector` to specify the checkbox.
* `uncheck`: Unchecks a checkbox (identified by a CSS selector). Requires a `selector` to specify the checkbox.
* `select`: Selects an option from a select box (identified by a CSS selector). Requires a `selector` to specify the select box.
* `wait`: Pauses execution for a specified amount of time. Requires a `value` representing the number of milliseconds to wait.
* `hotkey`: Simulates pressing a key or a combination of keys. Requires a `value` specifying the key or key combination.
* `assert_visible`: Asserts that an element (identified by a CSS selector) is visible. Requires a `selector` to specify the element.
* `assert_not_visible`: Asserts that an element (identified by a CSS selector) is not visible. Requires a `selector` to specify the element.
* `assert_text`: Asserts that the text content of an element (identified by a CSS selector) matches a specified value. Requires a `selector` to specify the element and a `value` to compare against.
* `assert_is_empty`: Asserts that the text content of an element (identified by a CSS selector) is empty. Requires a `selector` to specify the element.
* `assert_is_not_empty`: Asserts that the text content of an element (identified by a CSS selector) is not empty. Requires a `selector` to specify the element.
* `assert_input_value`: Asserts that the value of an input field (identified by a CSS selector) matches a specified value. Requires a `selector` to specify the input field and a `value` to compare against.
* `assert_checked`: Asserts that a checkbox (identified by a CSS selector) is checked. Requires a `selector` to specify the checkbox.
* `assert_not_checked`: Asserts that a checkbox (identified by a CSS selector) is not checked. Requires a `selector` to specify the checkbox.
* `assert_selected`: Asserts that a specific value is selected in a select box (identified by a CSS selector). Requires a `selector` to specify the select box.
* `assert_url`: Asserts that the current URL matches a specified value. Requires a `value` representing the expected URL.
* `undefined`: Represents an unknown yet action.

### Required Fields Summary <a href="#h_ffd4c45137" id="h_ffd4c45137"></a>

| Action Type           | Required Fields             |
| --------------------- | --------------------------- |
| `goto`                | `text`, `value`             |
| `click`               | `text`, `selector`          |
| `fill`                | `text`, `selector`, `value` |
| `check`               | `text`, `selector`          |
| `uncheck`             | `text`, `selector`          |
| `select`              | `text`, `selector`          |
| `wait`                | `text`, `value`             |
| `hotkey`              | `text`, `value`             |
| `assert_visible`      | `text`, `selector`          |
| `assert_not_visible`  | `text`, `selector`          |
| `assert_text`         | `text`, `selector`, `value` |
| `assert_is_empty`     | `text`, `selector`          |
| `assert_is_not_empty` | `text`, `selector`          |
| `assert_input_value`  | `text`, `selector`, `value` |
| `assert_checked`      | `text`, `selector`          |
| `assert_not_checked`  | `text`, `selector`          |
| `assert_selected`     | `text`, `selector`          |
| `assert_url`          | `text`, `value`             |
| `undefined`           | `text`                      |
