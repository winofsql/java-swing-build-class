# java-swing-build-class

![image](https://user-images.githubusercontent.com/1501327/184102429-6db56e9b-2cd3-4c4d-aec2-5b0d67ff5a6f.png)

![image](https://user-images.githubusercontent.com/1501327/184102809-ba46b88b-5056-4b5a-831d-4d668bc13205.png)

![image](https://user-images.githubusercontent.com/1501327/184103061-360b11d2-d6f6-4b7c-b11d-66ee6720e435.png)

![image](https://user-images.githubusercontent.com/1501327/184103234-565d2c20-4c74-4e13-a3f0-1ea65fcb3857.png)

```java
public class MyClass {

    private String title;

    public String getTitle() {
        return title;
    }

    public void setTitle(String title) {
        this.title = title;
    }

    public MyClass() {
    }

}
```

```java
        myClass = new MyClass();
        myClass.setTitle("処理開始");
        String title = myClass.getTitle();
        System.out.println(title);
```

## クラスメソッドの作成
```java
        myClass = new MyClass();
        myClass.setTitle("処理開始");
        String title = myClass.getTitle();
        // System.out.println(title);
        MyClass.print(title);
```

![image](https://user-images.githubusercontent.com/1501327/184263087-b3582ad6-2ab1-4c3b-aa95-8df57e87baab.png)

```java
public class MyClass {

    private String title;

    public String getTitle() {
        return title;
    }

    public void setTitle(String title) {
        this.title = title;
    }

    public MyClass() {
    }

    // ********************************
    // ★ クラスメソッド ★
    // ********************************
    public static void print(String value) {
        System.out.println(value);
    }
}
```

## launch.json の変更
![image](https://user-images.githubusercontent.com/1501327/184264884-46a1ef6e-fa4d-45c5-9d41-cff8089de3c4.png)

```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "type": "java",
            "name": "Launch Current File",
            "request": "launch",
            "mainClass": "${file}",
            "console": "internalConsole",
        }
    ]
}
```

![image](https://user-images.githubusercontent.com/1501327/184265102-05170a9e-6e3a-423a-8f1d-2a198a29582c.png)

## 続行

![image](https://user-images.githubusercontent.com/1501327/184265172-2bb796f8-f8d5-4213-80f3-303db7bd5a05.png)

