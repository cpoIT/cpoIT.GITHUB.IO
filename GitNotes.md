Git is a map of keys and values;
# SHA-1 (Secure Hash Algorithm 1)

SHA-1 (Secure Hash Algorithm 1) is a cryptographic hash function which takes an input and produces a 160-bit (20-byte) hash value known as a message digest - typically rendered as a hexadecimal number, 40 digits long.

It is practically impossible for two SHA-1 files to collide (i.e., 2 different files to have the same SHA-1 and be mixed up).

To get a SHA-1: echo "Hello World" | git hash-object --stdin
Output: 557db03de997c86a4a028e1ebd3a1ceb225be238

The first 2 numbers are the folder name and the remaining letters/numbers are the file name

To add a SHA-1 to a repository: echo "Hello World" | git hash-object --stdin -w

Initialize repository: git init;

Open repository: open .git;

Type of git file: git cat-file 557db03de997c86a4a028e1ebd3a1ceb225be238 -t
Output: blob
Blob (Binary Large OBject)

Type of git file: git cat-file 557db03de997c86a4a028e1ebd3a1ceb225be238 -p
Output: Hello World
