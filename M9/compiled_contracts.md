
# Team 12 - M9 - Method Contracts



## Nathan Lai
`agilepuppers.cleanwater.controller.RegisterScreen->handleRegister()`

**Signature**: `@FXML private void handleRegister()`

**Preconditions**: Current screen is `RegisterScreen`. New user has entered in a unique username, a password, and authorization level.

**Postconditions**: Upon successful registration, a new `UserAccount` is created for the user. The new user is then logged in and the screen changes to the `HomeScreen`. Else the screen stays on `RegisterScreen` if a new user could not be created.

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

## Cal Stephens

`agilepuppers.cleanwater.model.TextDatabase->queryAllEntries()`

**Signature**: `public List<T> queryAllEntries() throws IOException`

**Preconditions**: The TextDatabase must be initialized with a file path and a model factory.

**Postconditions**: If the specified file doesn't exist or cannot be accessed, an `IOException` will be thrown. Otherwise, the method will return a List of model objects as parsed by the database's model factory.

## Jeremy Winter
`agilepuppers.cleanwater.controller.LoginScreen->validate()`

**Signature**: `private UserAccount validate(String username, String password)`

**Preconditions**: Current screen is `LoginScreen`. This method should only be called by `handleLogin()`.

**Postconditions**: Upon successful login, `handleLogin` receives the proper user account and sets that as the current user. Otherwise, an error message is displayed. 
