
### About ME

**1. Introduce yourself.**  
My name is Vyshnave, and I am a passionate front-end developer with over three years of experience in web development. I have more than two years of specialized experience in React, creating responsive and dynamic web applications. My expertise extends to Next.js and Three.js, where I continue to explore and integrate advanced features into my projects.

**2. Do you own a personal computer?**  
Yes, I own a personal computer which I use for all my development work.

**3. Describe your development environment. (Your OS, IDE, Editor, and Config manager if any)**  
I work on a macOS (macOS Ventura). My primary IDE is Visual Studio Code, which I use for most of my coding tasks. I also have experience with WebStorm. My configuration management is handled through Git, and I use Homebrew for package management.

### Social Profile

**1. Your StackOverflow Profile URL.**

**2. Personal website, blog, or something you want us to see.**  
[\[git\]](https://github.com/vyshnave1997)
[\[Portfolio\]](https://vyshnave-portfolio.netlify.app/)



### The Real Stuff

**1. Which all programming languages are installed on your system.**  
On my system, I have the following programming languages installed:
- JavaScript/Node.js


**2. Write a function that takes a number and returns a list of its digits in an array.**

```javascript
function numberToDigitsArray(num) {
    return Array.from(String(num), Number);
}


console.log(numberToDigitsArray(12345)); 

// Output: [1, 2, 3, 4, 5]
```

**3. Remove duplicates of an array and return an array of only unique elements.**

```javascript
function removeDuplicates(arr) {
    return [...new Set(arr)];
}


console.log(removeDuplicates([1, 2, 2, 3, 4, 4, 5])); 

// Output: [1, 2, 3, 4, 5]
```

**4. Write a function that translates a text to Pig Latin and back.**

```javascript
function translateToPigLatin(text) {
    return text.split(' ').map(word => {
        return word.slice(1) + word[0] + 'ay';
    }).join(' ');
}

console.log(translateToPigLatin("The quick brown fox")); // 

Output: "Hetay uickqay rownbay oxfay"
```

**5. Write a function that rotates a list by `k` elements.**

```javascript
function rotateArray(arr, k) {
    k = k % arr.length;
    for (let i = 0; i < k; i++) {
        arr.push(arr.shift());
    }
    return arr;
}

// Example usage:
console.log(rotateArray([1, 2, 3, 4, 5, 6], 2)); // Output: [3, 4, 5, 6, 1, 2]
```

**Explanation:**  
The `rotateArray` function rotates the array in place without creating a copy. It moves elements from the front to the back, `k` times, resulting in a rotated array. The number of swap or move operations needed is `k`.

**Thank you **