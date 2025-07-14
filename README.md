# 🟢 Cơ Bản (Basic)

## 📂 Array Operations

### Bài 1: Tìm phần tử lớn nhất và nhỏ nhất trong mảng

Viết hai hàm:

- `findMax(arr: number[]): number` – Trả về phần tử lớn nhất.
- `findMin(arr: number[]): number` – Trả về phần tử nhỏ nhất.

**Ví dụ:**

```ts
findMax([1, 5, 3, 9, 2]); // 9
findMin([1, 5, 3, 9, 2]); // 1
```

---

### Bài 2: Tính tổng và trung bình của mảng

Viết hai hàm:

- `arraySum(arr: number[]): number` – Trả về tổng các phần tử.
- `arrayAverage(arr: number[]): number` – Trả về giá trị trung bình.

**Ví dụ:**

```ts
arraySum([4, 7, 1, 3]); // 15
arrayAverage([4, 7, 1, 3]); // 3.75
```

---

### Bài 3: Đảo ngược mảng và kiểm tra palindrome

Viết hai hàm:

- `reverseArray(arr: number[]): number[]` – Trả về mảng đảo ngược.
- `isPalindrome(arr: number[]): boolean` – Trả về true nếu mảng là palindrome.

**Ví dụ:**

```ts
reverseArray([1, 2, 3]); // [3, 2, 1]
isPalindrome([1, 2, 3, 2, 1]); // true
```

---

### Bài 4: Loại bỏ trùng lặp và tìm phần tử xuất hiện nhiều nhất

Viết hai hàm:

- `removeDuplicates(arr: number[]): number[]` – Trả về mảng không có phần tử trùng.
- `findMostFrequent(arr: number[]): number` – Trả về phần tử xuất hiện nhiều nhất.

**Ví dụ:**

```ts
removeDuplicates([1, 2, 2, 3, 1, 4]); // [1, 2, 3, 4]
findMostFrequent([1, 2, 2, 3, 2]); // 2
```

---

### Bài 5: Tìm cặp có tổng cho trước và xoay mảng

Viết hai hàm:

- `twoSum(arr: number[], target: number): [number, number] | null` – Trả về cặp có tổng bằng target.
- `rotateArray(arr: number[], k: number): number[]` – Xoay mảng sang phải k bước.

**Ví dụ:**

```ts
twoSum([2, 7, 11, 15], 9); // [2, 7]
rotateArray([1, 2, 3, 4, 5], 2); // [4, 5, 1, 2, 3]
```

---

## 📂 String Manipulation (11 bài)

### Bài 6: Đảo ngược chuỗi và kiểm tra palindrome chuỗi

Viết hai hàm:

- `reverseString(s: string): string`
- `isPalindromeString(s: string): boolean`

**Ví dụ:**

```ts
reverseString('hello'); // "olleh"
isPalindromeString('level'); // true
```

---

### Bài 7: Đếm ký tự và tìm ký tự không lặp đầu tiên

Viết hai hàm:

- `countCharacters(s: string): Record<string, number>` – Trả về số lần xuất hiện từng ký tự.
- `firstNonRepeatingChar(s: string): string | null` – Trả về ký tự không lặp đầu tiên hoặc null.

**Ví dụ:**

```ts
countCharacters('aabccc'); // { a: 2, b: 1, c: 3 }
firstNonRepeatingChar('aabbc'); // "c"
```

---

### Bài 8: Kiểm tra anagram và tìm chuỗi con không lặp dài nhất

Viết hai hàm:

- `isAnagram(s1: string, s2: string): boolean`
- `longestUniqueSubstring(s: string): string`

**Ví dụ:**

```ts
isAnagram('listen', 'silent'); // true
longestUniqueSubstring('abcabcbb'); // "abc"
```

---

### Bài 9: Nén và giải nén chuỗi (run-length encoding)

Viết hai hàm:

- `compressString(s: string): string` – Nén chuỗi theo số lượng ký tự liên tiếp.
- `decompressString(s: string): string` – Giải nén chuỗi đã được nén.

**Ví dụ:**

```ts
compressString('aaabbc'); // "a3b2c1"
decompressString('a3b2c1'); // "aaabbc"
```

---

### Bài 10: Sinh hoán vị, kiểm tra subsequence và tìm pattern (KMP)

Viết ba hàm:

- `getPermutations(s: string): string[]` – Trả về tất cả hoán vị của chuỗi.
- `isSubsequence(s: string, t: string): boolean` – Kiểm tra s có phải subsequence của t không.
- `findPattern(text: string, pattern: string): number[]` – Trả về các vị trí khớp bằng thuật toán KMP.

**Ví dụ:**

```ts
getPermutations('abc'); // ["abc", "acb", "bac", "bca", "cab", "cba"]
isSubsequence('abc', 'ahbgdc'); // true
findPattern('ababcabcabab', 'ab'); // [0, 2, 5, 9]
```

---

### Bài 11: Bubble Sort, Selection Sort, Insertion Sort

Viết ba hàm sắp xếp mảng số nguyên theo thứ tự tăng dần, mỗi hàm sử dụng một thuật toán khác nhau:

- `bubbleSort(arr: number[]): number[]` - Thuật toán nổi bọt: lặp qua mảng nhiều lần, hoán đổi cặp phần tử liền kề nếu phần tử phía trước lớn hơn phía sau. Dừng khi không còn phần tử nào cần hoán đổi.

- `selectionSort(arr: number[]): number[]` - Thuật toán chọn: duyệt qua mảng, tại mỗi bước tìm phần tử nhỏ nhất trong phần còn lại và hoán đổi với phần tử hiện tại.

- `insertionSort(arr: number[]): number[]` - Thuật toán chèn: duyệt từng phần tử và chèn vào đúng vị trí trong phần đã sắp xếp bên trái.

- Yêu cầu: Không sử dụng .sort() có sẵn.

**Ví dụ:**

```ts
bubbleSort([5, 3, 1, 4, 2])      // [1, 2, 3, 4, 5]
selectionSort([29, 10, 14, 37]) // [10, 14, 29, 37]
insertionSort([4, 3, 2, 10])     // [2, 3, 4, 10]
```

---

### Bài 12: Linear, Binary, Binary Recursive Search

Viết các hàm tìm kiếm một phần tử trong mảng số nguyên đã được sắp xếp theo thứ tự tăng dần:

- `linearSearch(arr: number[], target: number): number` - Duyệt từ đầu đến cuối mảng. Trả về chỉ số đầu tiên có giá trị bằng target, nếu không tìm thấy thì trả về -1.

- `binarySearch(arr: number[], target: number): number` - Áp dụng thuật toán tìm kiếm nhị phân không đệ quy. Chia đôi mảng mỗi bước để thu hẹp phạm vi tìm kiếm. Trả về chỉ số phần tử hoặc -1 nếu không tồn tại.

- `binarySearchRecursive(arr: number[], target: number, left: number, right: number): number` - Tìm kiếm nhị phân sử dụng đệ quy. Bắt đầu với left = 0, right = arr.length - 1.
Trả về chỉ số nếu tìm thấy, ngược lại trả về -1.

**Ví dụ:**
```ts
linearSearch([1, 3, 5], 5)             // 2
binarySearch([1, 2, 3, 4], 4)          // 3
binarySearchRecursive([10, 20], 20, 0, 1) // 1
```
