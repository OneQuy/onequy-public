# AppState in React Native

I was on my way to fix a bug when I learned more deeply about `AppState` in React Native. According to the official docs, there are 3 states:  
- **Active** (both Android & iOS)  
- **Background** (both Android & iOS)  
- **Inactive** (iOS only)  

But the bug I faced was caused by the **`background` state not being triggered** when the app was swiped up to quit completely on older iPhone versions.  
In those cases, it only triggers `inactive`.

So, if you want a simple way to handle app state:

**On iOS:**  
- `active`  
- `inactive`  

**On Android:**  
- `active`  
- `background`  

That's it.

---

Let me know if you want to post it somewhere and need a tweet-sized version too!