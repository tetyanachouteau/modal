# modal

Library to add modal to the HRNet project

## Install

```bash
npm install --save @zhabchyk/modalhrnet
```

## usage 

### configuration

```jsx
const customConfig = {
    buttons: [
        {
            label: 'Home',
            className: styles.buttonPurple, // Purple button style from CSS module
            action: closeModal // Action to close modal
        },
        {
            label: 'List-employees',
            className: styles.buttonGreen,
            action: goList
        }
    ],
    title: "Confirmation",
    onCloseIcon: closeModal
};
```

Parameters :
* buttons: add button to the end of the modal
    * label: label of the button
    * className: class of the button
    * action: action when button is clicked
* title: title of the modal
* onCloseIcon: action when click to the close icon of the modal

### component 

```jsx
<Modal show={isModalVisible} config={customConfig}>
    {<h1>Employee Created</h1>

    <Callout
        title={"Success"}
        type={"success"}
    >

        <p> 💫 Validation: The task of validating the form has been successfully completed.</p>
        <p>All required fields have been correctly validated according to the specified criteria.</p>
    </Callout>}
</Modal>

```

## License

MIT © [tetyanachouteau](https://github.com/tetyanachouteau)
