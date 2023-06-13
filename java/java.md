```java
public class _Quiz_06 {

    public static String gethiddenmethod(String name, int num) {
        String hidden = name.substring(0, num);
        for (int i = 0; i < name.length() - num; i++) {

            hidden += "*";


        }

        return hidden;
    }

    public static void main(String[] args) {

        String name = "강민규";
        String id = "990130-1234567"; // 14개 8개부터 지워 하이픈 남기고 그러면 6개 남잖아 그만큼 별을 추가
         String phone = "010-4616-7626";
        System.out.println("이름 : " + gethiddenmethod(name, 1));
        System.out.println("주민등록 번호 : " + gethiddenmethod(id, 8));
        System.out.println("전화번호 : "+ gethiddenmethod(phone, 9));
    }

}
```