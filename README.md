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
