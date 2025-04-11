- how to delete branch locally

```sh
git branch -d branch_name

git branch -D branch_name
```

- how to delete branch remotely

```sh
git push origin --delete branch_name
```

# Annotated vs Lightweight

Tags in Git are references to specific points in your repository's history, primarily used for marking release points (v1.0, v2.1, etc.). Git offers two types of tags with different characteristics:

# Annotated Tags

What they are:

- Full-fledged Git objects stored in the database

- Contain comprehensive metadata about the tag

Key features:

- Store the tagger's name and email

- Include the date of tagging

- Contain a descriptive message (like commit messages)

- Can be cryptographically signed with GPG

# Lightweight Tags

What they are:

Simple pointers to specific commits

Just a name referencing a commit hash

Key features:

No additional metadata stored

- Don't contain tagger information or dates

- Can't be signed

- Very lightweight (hence the name)

When to use:

- Temporary or private tags

- Quick local references

- When you don't need historical tracking

# When To Use Rebase

1- Maintaining a linear history: Rebase helps keep the project history clean by avoiding unnecessary merge commits

2- Updating a feature branch with the latest main branch changes: Rebase applies the feature branch's commits on top of the latest main branch to avoid conflicts during later merges.

# How To List Tags

- List all tags:

```sh
git tag
```

- List tags with details (annotated):

```sh
git show <tag-name>
```

# How To Delete Tags

- Locally

```sh
 git tag -d v1.0
```

- Remotely

```sh
 git push origin --delete v1.0
```

# Image

<img src="pexels-photo-2071882.jpeg" alt="Cat Image" width="400"/>
