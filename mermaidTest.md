···
1graph TD2A[Android Handler] -->B(Handler)3B -->C[Message]4B -->D[Message Queue]5C -->E{是否有Looper}6E -->|是|F[子线程Looper]7E -->|否|G[主线程Looper]8F -->END(结束)9G -->END(结束)
···
