# Checkbox 2

<input type="checkbox" id="myCheckbox"> Remember me

<script input="checkbox2">
    document.addEventListener('DOMContentLoaded', (event) => {
        const checkbox = document.getElementById('myCheckbox');

        // Load the saved state from local storage
        const isChecked = localStorage.getItem('checkboxState') === 'true';
        checkbox.checked = isChecked;

        // Save the state to local storage whenever it changes
        checkbox.addEventListener('change', () => {
            localStorage.setItem('checkboxState', checkbox.checked);
        });
    });
</script>

- [ ] Test


