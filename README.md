# 🔤 clsString – C++ String Utility Class

A lightweight, header-only C++ class that wraps common string operations in one place. Every function is available both as a **static method** (pass any string) and as an **object method** (works on the stored value).

---

## ✨ Features

- **🔠 Case Handling**
  - Uppercase / lowercase the whole string
  - Uppercase / lowercase the first letter of each word
  - Invert the case of every letter

- **🔢 Counting**
  - Length, words, vowels
  - Capital / small letters
  - A specific letter (with or without case matching)

- **✂️ Splitting & Joining**
  - Split by any delimiter into a `vector<string>`
  - Join a vector or array back into one string

- **🧹 Cleaning**
  - Trim left / right / both
  - Remove punctuation

- **🔁 Transforming**
  - Reverse word order
  - Replace a word (with or without case matching)

---

## 🚀 Usage

```cpp
#include "clsString.h"

int main()
{
    // Object style
    clsString S("  hello world from c++  ");
    S.Trim();
    S.UpperFirstLetterOfEachWord();
    cout << S.GetValue() << endl;          // Hello World From C++

    // Static style
    cout << clsString::CountWords("one two three") << endl;    // 3
    cout << clsString::ReverseWordsInString("a b c") << endl;  // c b a
}
```

---

## 🛠️ Compile

```bash
g++ main.cpp -o main
./main
```

> Uses `<bits/stdc++.h>`, so it builds with **g++ / MinGW**. For MSVC, replace it with the specific standard headers.

---

🚨 **Feel free to fork, modify, or use this as a learning resource!** 🛠️
