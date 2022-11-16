useEffect

1. Cập nhật lại state
2. Cập nhật DOM(mutated)
3. Render lại UI
4. Gọi cleanup nếu deps thay đổi
5. Gọi useEffect callback

---

+) Side Effects
+) Events:Add/remove event listener
+) Observer pattern:Subscribe/unsubscribe
+) Closure
+) Timers:setInterval,setTimeout,clearInterval,clearTimeout
+) useState
+) Mounted unmounted
+) ===
+) Call API

1. Update DOM
   F8 blog title
2. Call API
3. Listen DOM events
   Scroll
   Resize
4. Cleanup
   Remove listener/Unsubscribe
   Clear timer

---

a. useEffect(callback)
b. useEffect(callback,[])
c. useEffect(callback,[deps])

---

1. useEffect(callback)
   – Gọi callback mỗi khi component re-render
   – Gọi callback sau khi component thêm element vào DOM
2. useEffect(callback,[])

- Chỉ gọi callback 1 lần sau khi component mounted

3. useEffect(callback,[deps])

- Callback sẽ được gọi lại mỗi khi deps thay đổi

---

1. Callback luôn được gọi sau khi componet mounted
2. Cleanup function luôn được gọi trước khi conponent unmounted
3. Cleanup function luôn được gọi trước khi callback được gọi (trừ lần mounted)
