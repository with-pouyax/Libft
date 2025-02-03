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
