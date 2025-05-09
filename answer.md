# answers.md

## About You

### 1. Introduce yourself.
Hi, I'm Vyshnave, a passionate Frontend Developer with 4 years of experience building responsive and interactive web applications. I specialize in React, Next.js, and modern web technologies. I enjoy creating smooth user experiences and exploring creative ways to solve complex problems.

### 2. Do you own a personal computer?
Yes, I use my personal computer for development and learning new technologies.

### 3. Describe your development environment. (Your OS, IDE, Editor and Config manager if any)
- **OS**: Windows 11
- **IDE/Editor**: Visual Studio Code with extensions for ESLint, Prettier, GitLens, Tailwind CSS IntelliSense
- **Terminal**: PowerShell & Ubuntu via WSL2
- **Version Control**: Git
- **Config Manager**: `.editorconfig`, ESLint, Prettier, `.gitconfig`

---

## Social Profile

### 1. Your StackOverflow Profile URL.


### 2. Personal website, blog or something you want us to see.
[https://github.com/vyshnave1997](https://github.com/vyshnave1997)

---

## The Real Stuff

### 1. Which all programming languages are installed on your system?
- JavaScript (Node.js)
- TypeScript
- Python
- Bash (via WSL)
- HTML/CSS (in browser/dev tools)

---

### 2. Write a function that takes a number and returns a list of its digits in an array.

```javascript
function getDigits(num) {
  return num.toString().split('').map(Number);
}


console.log(getDigits(12345)); // Output: [1, 2, 3, 4, 5]


3. Remove duplicates of an array and return an array of only unique elements.

function uniqueArray(arr) {
  return [...new Set(arr)];
}


console.log(uniqueArray([1, 2, 2, 3, 4, 4, 5])); // Output: [1, 2, 3, 4, 5]

4. Write a function that translates text to Pig Latin and back.

function toPigLatin(text) {
  return text
    .split(' ')
    .map(word => word.slice(1) + word[0] + 'ay')
    .join(' ');
}

function fromPigLatin(pigText) {
  return pigText
    .split(' ')
    .map(word => {
      const noAy = word.slice(0, -2); 
      return noAy.slice(-1) + noAy.slice(0, -1);
    })
    .join(' ');
}


const pig = toPigLatin("The quick brown fox");
console.log(pig); 
console.log(fromPigLatin(pig)); 
5. Write a function that rotates a list by k elements (without creating a copy).
javascript
Copy
Edit
function rotateInPlace(arr, k) {
  const n = arr.length;
  k = k % n;
  reverse(arr, 0, k - 1);
  reverse(arr, k, n - 1);
  reverse(arr, 0, n - 1);
  return arr;
}

function reverse(arr, start, end) {
  while (start < end) {
    [arr[start], arr[end]] = [arr[end], arr[start]];
    start++;
    end--;
  }
}


console.log(rotateInPlace([1, 2, 3, 4, 5, 6], 2)); // Output: [3, 4, 5, 6, 1, 2]



