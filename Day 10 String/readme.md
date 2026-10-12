

# 🧵 String Operations in C

This repository contains **beginner-friendly C programs** that demonstrate **basic string handling techniques** in the C programming language.
These examples will help you understand how to **declare, input, print, and measure strings** using different methods.

---

## 🧠 What is a String?

A **string** in C is a sequence of **characters** terminated by a **null character (`'\0'`)**.
Unlike other languages, C does not have a dedicated string type — strings are simply arrays of characters.

**Example:**

```c
char name[6] = "HELLO";
```

| Index | 0 | 1 | 2 | 3 | 4 | 5  |
| ----- | - | - | - | - | - | -- |
| Value | H | E | L | L | O | \0 |

---

## 📂 Programs in This Project

### 🟦 1. **string_length_strlen.c**

**Concept:** Calculate string length using the built-in `strlen()` function.

```c
#include <stdio.h>
#include <string.h>

int main() {
    char s[101];
    fgets(s, 101, stdin);

    int size = strlen(s);
    printf("%d", size);
    return 0;
}
```

**Example Input:**

```
Programming
```

**Example Output:**

```
12
```

🧩 *The `strlen()` function counts characters until it reaches the null terminator.*

---

### 🟩 2. **string_length_manual.c**

**Concept:** Find string length **manually** using a loop.

```c
#include <stdio.h>

int main() {
    char s[101];
    fgets(s, 101, stdin);
    int count = 0;

    for (int i = 0; s[i] != '\0'; i++) {
        count++;
    }

    printf("%d", count);
    return 0;
}
```

**Example Input:**

```
C Programming
```

**Example Output:**

```
14
```

🧠 *Manually iterates through each character until the null character `'\0'`.*

---

### 🟨 3. **string_basic.c**

**Concept:** Declare and print a string in C.

```c
#include <stdio.h>

int main() {
    char s[6] = "HELLO";
    printf("%s", s);
    return 0;
}
```

**Example Output:**

```
HELLO
```

💡 *The null terminator `'\0'` is automatically added at the end of the string.*

---

### 🟧 4. **string_input_fgets.c**

**Concept:** Read a string from input using `fgets()` and print it.

```c
#include <stdio.h>
#include <string.h>

int main() {
    char s[25];
    fgets(s, 24, stdin);
    printf("%s", s);
    return 0;
}
```

**Example Input:**

```
Hello World!
```

**Example Output:**

```
Hello World!
```

⚙️ *Unlike `gets()`, `fgets()` is safe — it prevents buffer overflow.*

---

### 🟥 5. **string_input_scanf.c**

**Concept:** Input a string using `scanf()` and print it.

```c
#include <stdio.h>

int main() {
    char s[10];
    scanf("%s", s);
    printf("%s", s);
    return 0;
}
```

**Example Input:**

```
Hello
```

**Example Output:**

```
Hello
```

⚠️ *`scanf()` stops reading when it encounters whitespace.*

---

### 🟪 6. **char_array_input.c**

**Concept:** Input and print characters one by one.

```c
#include <stdio.h>

int main() {
    char arr[5];
    for (int i = 0; i < 5; i++) {
        scanf("%c", &arr[i]);
    }
    for (int i = 0; i < 5; i++) {
        printf("%c", arr[i]);
    }
    return 0;
}
```

**Example Input:**

```
HELLO
```

**Example Output:**

```
HELLO
```

🔍 *Demonstrates low-level string input using character arrays.*

---

## 🔑 Key Concepts

| Concept            | Description                                            |
| ------------------ | ------------------------------------------------------ |
| String Declaration | Strings are arrays of characters ending with `'\0'`.   |
| String Input       | Use `scanf()`, `gets()` (unsafe), or `fgets()` (safe). |
| String Output      | `printf("%s", str)` prints the entire string.          |
| String Length      | Count characters until `'\0'` or use `strlen()`.       |
| Character Array    | Each element stores one character, including spaces.   |

---

## ⚙️ How to Compile and Run

```bash
# Compile
gcc string_length_strlen.c -o string_length

# Run
./string_length
```

* Replace the filename to test other programs.
* Use a **C99 compatible compiler** for best results.

---

## 🏁 Summary

* Strings are essential for **text manipulation** in C.
* Always ensure **enough space** for the null character.
* Prefer **fgets()** over **gets()** for safer input.
* You can measure string length manually or using `strlen()`.

---



# Author

## **Engr. Md Monjur Bakth Mazumder**

🎓 **Secondary School Certificate (SSC) from [Shah Helal High School](https://www.shahhelalhs.edu.bd/)**

🎓 **Diploma in Computer Science and Technology from [Moulvibazar Polytechnic Institute (MPI)](https://mpi.moulvibazar.gov.bd/)**

🎓 **BSc in Computer Science & Engineering (CSE)** _(Ongoing)_ **at [Sylhet International University (SIU)](https://siu.edu.bd/)**

---

## Support the Project

If you found this repository helpful, please consider giving it a **⭐ Star**. It helps others discover the project and motivates future development.

---


## Connect with Me

### Professional Profiles

| Platform | Link |
|:---|:---|
| Portfolio | [monjurmbm404.github.io](https://monjurmbm404.github.io) |
| GitHub | [monjurmbm404](https://github.com/monjurmbm404) |
| LinkedIn | [monjurmbm404](https://www.linkedin.com/in/monjurmbm404) |
| Medium | [@monjurmbm404](https://medium.com/@monjurmbm404) |

### Competitive Programming

| Platform | Link |
|:---|:---|
| Codeforces | [monjurmbm404](https://codeforces.com/profile/monjurmbm404) |
| CodeChef | [monjurmbm404](https://www.codechef.com/users/monjurmbm404) |
| LeetCode | [monjurmbm404](https://leetcode.com/u/monjurmbm404) |
| VJudge | [monjurmbm404](https://vjudge.net/user/monjurmbm404) |

### Social Media

| Platform | Link |
|:---|:---|
| Facebook | [monjurmbm404](https://www.facebook.com/monjurmbm404) |
| X (Twitter) | [@monjurmbm404](https://x.com/monjurmbm404) |
| YouTube | [@monjurmbm404](https://youtube.com/@monjurmbm404) |

### Contact Information

| Type | Email |
|:---|:---|
| Professional | [monjurmbm404@gmail.com](mailto:monjurmbm404@gmail.com) |