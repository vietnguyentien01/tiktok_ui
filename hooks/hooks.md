Hook - Gắn (gắn vào component)
Hooks duợc thêm vào React từ phiên bán 16.8.0

import {
useState,
useEffect,
uselayoutEffect,
useRef,
useCallback,
useMemo,
usekeducer,
useContext,
useImperativetandte,
useDebugValue,
}from 'react'

1. Chỉ dùng cho function component
2. Component đơn giản và trở nên dễ hiểu
   - Không bị chia logic ra như methods trong lifecycle của Class Component
   - Không cần sử dụng "this"
3. Sử dụng Hooks khi nào?

   - Dự án mới => Hooks
   - Dự án cũ:

     - Component mới => Function component + Hooks
     - Component cũ => Giữ nguyên, có thời gian tối ưu sau

   - Logic nghiệp vụ cần sử dụng các tính chất của OOP => Class component

4. Người mới nên bắt đầu với Function hay Class component?
5. Có kết hợp sử dụng Function component & Class component được không?
   - Được
