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
![image](https://user-images.githubusercontent.com/1501327/184263883-d3ebbc67-7835-484a-8139-6a6292b15a1c.png)

```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "type": "java",
            "name": "Launch Current File",
            "request": "launch",
            "mainClass": "${file}"
        },
        {
            "type": "java",
            "name": "Launch WinMain",
            "request": "launch",
            "mainClass": "WinMain",
            "console": "internalConsole",
            "projectName": "java-swing-build-class_dbd10125"
        }
    ]
}
```

![image](https://user-images.githubusercontent.com/1501327/184264165-cc4fb110-72c5-43b4-8618-1d4716178e99.png)
