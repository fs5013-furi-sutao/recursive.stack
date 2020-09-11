# スタック操作の再帰呼び出し
スタックに対して再帰呼び出しで Pop と Shift を繰り返すコード

基本情報技術者試験の平成31年春期 午前問6 の問題を引用している。

変数 A, B, C はいずれも、スタックのデータ構造です。

```java
void f() {
    if (A.isEmpty()) {
        // nothing
    } else {
        C.push(A.pop());
        f();
        B.push(C.pop());
    }
}
```

再帰呼び出しの動きを表すと、以下のイメージになる。

![スタック操作の再帰呼び出しを可視化](./explain_image/stack_pop_push_flow.png)  
