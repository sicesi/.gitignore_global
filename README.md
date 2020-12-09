# Our Common Global Gitignore File

## The Problem

Who wants to bloat the index with `Thumbs.db` & `.DS_Stores`?

Every time we start a new project, we have to make sure we will only commit relevant files to Git. After writing loads of exclusion rules for every new project, it became obvious there must be a better way. This is boring.

## The Solution

Turns out, there is a better way! We can use a `.gitignore_global` file that will apply to every Git repository on our system 🙌

Due to it's shared nature, this file is best suited for exclusion rules that have nothing to do with the project itself, but rather with your host OS, you IDE and other common file types.

## I'm in! How do I use it?

First, let's create the file and tell Git to use it:

- ### macOS

```bash
touch ~/.gitignore_global

git config --global core.excludesfile ~/.gitignore_global
```

- ### Windows

Go to your `C:\Users\{username}\` folder and create a `.gitignore_global` file.

Then run the following command:

```bash
git config --global core.excludesfile "%USERPROFILE%\.gitignore"
```

Now, copy paste the common rules we wrote together here and you are all set 😎

## Contributing

Of course, feel free to contribute to this shared file if you see something missing!
