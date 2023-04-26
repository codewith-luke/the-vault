When using docker by default it will make use of the root user. If you want to be able to allow other users to access and perform operations you can make use of groups.

Here you can create then use the new user:

```sh
useradd {user}
su - {user}
```

We then need to add this new user to the Docker Group use:

```
usermod -aG docker {user}
```

Then you would add you new user to the docker section. This will not allow them to do everything. So anything outside of sudo privileges. 
