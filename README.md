# Exercises for Git's Internal

A problem set for strengthen an understanding of Git's internals

## Steps

### 1. Clone this repository

Clone this repository to your machine (PC/laptop/etc).

### 2. Object types in Git

From lecture, we know that there are four types of Git objects

1. Blob
2. Commit
3. (annotated) tag
4. Tree

### 3. Content stored in an object

Given a Git object with a hash `22220e20fd799c1bcbee5f6940e9ccf3b9aebd41`,
we can view type of the object with the following command.

```console
$ git cat-file -t 22220e20fd799c1bcbee5f6940e9ccf3b9aebd41
blob
```

Similarly, we can get the size of the object by

```console
$ git cat-file -s 22220e20fd799c1bcbee5f6940e9ccf3b9aebd41
90
```

Lastly, with `-p` we can view the content stored in the object.

```console
$ git cat-file -p 22220e20fd799c1bcbee5f6940e9ccf3b9aebd41
# git-internal-exercises
A problem set for strengthen an understanding of Git's internals
```

### 4. The Blob object

The object we examined in the previous step is a blob object.
The content in this type of object is the content you see
in the file.

### 5. The Commit object

### 6. The Tag object

## Questions

### Question A: What is the type of object: HASH-VALUE ?

Use the command you learn in previous section, find the type of the object with
hash `HASH-VALUE`.

1. What is the command you use to find the answer?
2. What is the type of the object?
3. What is the size of the object?

### Question B: Find the hash of a file named git-list-pack

Use the command you learn in this homework, find the hash value
of the file named `git-list-pack`.

### Question C: Find the hash of a folder named scripts

Use the command you learn in this homework, find the hash value
of the object of a folder named `scripts`.

With this hash value, answer the following questions

- What is the type of this object?
- What is the size of this object?
- What are other hash values stored in this object? For each hash value
  What are its type, size and name.
