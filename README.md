# linux-file-permissions
Understand Linux file permissions, create a flowchart, and apply chmod.

# Understanding File Permissions

Let's start by understanding file permissions and how to read them. In Linux, permissions are divided into three categories: the owner, the group, and others. Each of these groups has specific access rights to a file or directory.

To make this clearer, let's look at an image that explains everything visually.

<img width="1400" height="788" alt="yxNrpKJ" src="https://github.com/user-attachments/assets/a06d5820-4dc9-48d3-9522-7f174ee09da7" />


# How to apply the chmod command in a Python file to make the permissions rwxrwxr-x ?

To change a file’s permissions in Linux using the chmod command, the general form is:

sudo chmod [permissions] [filename]

So, in our example, to apply rwxrwxr-x permissions to a file called linuxtask.py, we write:

sudo chmod 775 linuxtask.py

But why do we use 775?

The number 775 represents the permission set rwxrwxr-x. To understand this, let’s break it down:

Linux uses the following values for each permission:

-r (read) = 4

-w (write) = 2

-x (execute) = 1

| Entity     | Permissions | Binary | Sum               |
| ---------- | ----------- | ------ | ----------------- |
| **Owner**  | `rwx`       | 111    | 4 + 2 + 1 = **7** |
| **Group**  | `rwx`       | 111    | 4 + 2 + 1 = **7** |
| **Others** | `r-x`       | 101    | 4 + 0 + 1 = **5** |

# Flowchart for the previous example


<img width="771" height="1005" alt="Permissions are divided into 3 parts (1)" src="https://github.com/user-attachments/assets/def8c8d9-309f-4dab-9b7a-a3ecc14179b8" />


# Linux Implementation
The following image shows the implementation of changing file permissions using the chmod command in the Linux terminal.
<img width="1278" height="799" alt="Screenshot 2025-07-24 171800" src="https://github.com/user-attachments/assets/250caec3-8572-420e-84fb-5b15843aff36" />

