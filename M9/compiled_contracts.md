
# Team 12 - M9 - Contracts


## Ridoy Majumdar

`agilepuppers.cleanwater.controller.EditProfile->updateProfile()`

**Preconditions**:

       titleField.getText() != null && nameField.getText() != null
    && emailField.getText != null   && addressField.getText() != null

**Postconditions**:

       profile.title.equals(titleField.getText())
    && profile.name.equals(nameField.getText())
    && profile.email.equals(emailField.getText())
    && profile.address.equals(addressField.getText())

## Gabor Siffel

`agilepuppers.cleanwater.controller.LoginScreen->handleLogin()`

**Signature**: `@FXML private void handleLogin()`

**Preconditions**: Current screen is `LoginScreen`. Also, this method should only be called by JavaFX automatically when the user clicks the “Login” button

**Postconditions**: Current screen is either `HomeScreen` (on a successful login attempt) or remains on `LoginScreen` (on an unsuccessful login attempt); `App.current.user` is now set to the user that just logged in (if successful)
