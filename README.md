# libft


![Libft](https://user-images.githubusercontent.com/58959408/150704272-0d7b454d-2872-4695-aade-e5bc9c3b79aa.jpg)

# **libft - Custom C Standard Library Implementation**

Welcome to my **libft** repository! 🚀  
This project is my implementation of a subset of the **C Standard Library functions**, written in **C**, as part of the **42 School curriculum**.  
The library provides essential **memory management, string manipulation, character checking, and file descriptor operations**.  

---

## 📌 **Functions List & Detailed Descriptions**

### **1️⃣ Memory Functions**

1. **`ft_memset(void *s, int c, size_t n)`**  
   - Fills `n` bytes of the memory block pointed to by `s` with the byte `c`.  
   - Equivalent to `memset()` in `<string.h>`.  
   - Useful for initializing memory to a specific value.

2. **`ft_bzero(void *s, size_t n)`**  
   - Writes `n` bytes of zero (` `) to the memory block pointed to by `s`.  
   - Equivalent to `bzero()`, but deprecated in modern C in favor of `memset(s, 0, n)`.  
   - Used to initialize memory safely.

3. **`ft_memcpy(void *dest, const void *src, size_t n)`**  
   - Copies `n` bytes from `src` to `dest`.  
   - Does **not** handle overlapping memory regions.  
   - If overlapping is a concern, use `ft_memmove()`.

4. **`ft_memmove(void *dest, const void *src, size_t n)`**  
   - Similar to `ft_memcpy()`, but **handles overlapping memory regions**.  
   - Copies bytes in a way that prevents corruption of original data.

5. **`ft_memchr(const void *s, int c, size_t n)`**  
   - Scans the first `n` bytes of `s` to find the first occurrence of `c`.  
   - Returns a pointer to the byte if found, `NULL` otherwise.

6. **`ft_memcmp(const void *s1, const void *s2, size_t n)`**  
   - Compares two memory blocks byte by byte for `n` bytes.  
   - Returns `0` if they are identical, a positive or negative value otherwise.

7. **`ft_calloc(size_t count, size_t size)`**  
   - Allocates memory for `count` elements of `size` bytes each and initializes to zero.  
   - Unlike `malloc()`, ensures that the memory is set to `0` (safe allocation).

---
