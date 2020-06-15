## Django Cutom User
- Django ships with a built-in User model for authentication
- It's helpful to create a superuser that we can use to login to the admin and test out login/logout
- `USERNAME_FIELD = 'email'` will define that the email is what will be used to login
- `REQUIRED_FILEDS = ['username']` requires the user to setup a username when creating an account
- requirded functions `has_perm` and `has_module_perms` to setup a custom user
- a superuser will have administrative rights whereas a user will have usage rights 