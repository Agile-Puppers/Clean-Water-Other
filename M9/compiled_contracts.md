
# Team 12 ~ M9 ~ Contracts



### Gabor Siffel

**Signature**: `@FXML private void handleLogin()`

**Preconditions**: Current screen is `LoginScreen`. Also, this method should only be called by JavaFX automatically when the user clicks the “Login” button

**Postconditions**: Current screen is either `HomeScreen` (on a successful login attempt) or remains on `LoginScreen` (on an unsuccessful login attempt); `App.current.user` is now set to the user that just logged in (if successful)
