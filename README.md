# HTML-Form-Radio-Button

In HTML, a radio button is an interactive page element for selecting one option from multiple options. A radio button appears as an empty circle when unselected. When clicked with the mouse or selected with the keyboard, the circle fills in to indicate selection, A radio button is paired with a label (usually text or sometimes an image) — this is what the user is choosing when they select a particular radio button.

Radio buttons almost always appear in groups of two or more to represent related, mutually exclusive options. Within this group of options, a user may only select one at a time. This means that selecting a radio button deselects another selected button in the group. Also, users can’t deselect a radio button by clicking it. The only way to deselect a radio button is to select another option within the group.

Radio Buttons vs. Checkboxes
Radio buttons are similar to another common interactive element, the checkbox. The differences between these two are small but important to note: Whereas radio buttons let users select exactly one option per group, checkboxes let users choose (or “check”) one, multiple, or no options per group. Users can also deselect a checkbox by clicking it — radio buttons don’t allow this.

I’ll admit this isn’t the most thrilling topic. However, mixing up these two can cause serious confusion from visitors. So, be sure to use radio buttons for “Select one” menus, and save checkboxes for your “Select all that apply” menus or your one-off questions (i.e., “Check this box if…”).

Now that we understand the purpose of HTML radio buttons, let’s learn how to make them.

Here we have three <input> elements of type radio, with some new attributes as well. There’s also a new <label> element for each <input>. Let’s review each thing we added to the code.

First, the id attribute is a unique identifier for the <input> tag. It can be used as a CSS selector for the radio button element, and it also unites the button with its corresponding <label>.

As mentioned, radio buttons come in groups. Use the required name attribute to group together a set of related radio buttons. In the above example, all <input>s share the same value for name, so they are treated as part of the same group. This lets users only choose one option in a group at a time — try it out above.

Next, the value attribute represents a unique value for the radio button. Users don’t see it, but this is submitted to represent the chosen option. For example, if the form above was submitted with the “17 years or younger” item selected, the system processing the form would receive the value age=child. If the user does not select any radio button, no value will be sent. If the value attribute is missing for the selected option, the form will send the default value on.

Note that <input> tags only create the radio button element, not the label. To label a radio button, add a <label> element after the <input> element and insert a for attribute with the same value as the id of the associated <input> element. Then, write your label text in the <label> tag.

While using <label> isn’t strictly necessary, it’s considered a best practice for two reasons. First, the semantically rich <label> element makes your website more accessible for people using screen readers. It tells them which label is paired with which radio button. Second, the for attribute lets users select a radio button by clicking the label itself in addition to the button, making your form easier to use.

Finally, the <br> (line break) tags put each option on a new line. Try removing these tags in the example above to place all options on the same line.
