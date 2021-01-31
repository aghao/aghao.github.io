```mermaid
graph TD
A[Android Handler] -->B(Handler)
B -->C[Message]
B -->D[Message Queue]
C -->E{是否有Looper}
E -->|是|F[子线程Looper]
E -->|否|G[主线程Looper]
F -->END(结束)
G -->END(结束)
```
