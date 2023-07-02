# Homework_JavaCore_10
```public class JvmComprehension {  
  public static void main(String[] args) {  
    int i = 1;
// 1 Создается переменная i со значением 1 в Stack Memory  
    Object o = new Object();
// 2 Загрузка класса Object. Будет выделена память в heap. Вызван конструктор Object и ссылка кучи присвоена переменной o  
    Integer ii = 2;
// 3 Загрузка класса Integer. Будет выделена память в heap. Ссылка присвоена переменной ii 
    printAll(o, i, ii);
// 4 Выделен фрейм с новыми созданными переменными связанные с уже существующими ссылками или значениями. При выполнении операции - уничтожение фрейма и переменных, содержащих в нем  
    System.out.println("finished");
// 7 Выделен фрейм с созданием ссылки на объект String и выполнен метод печати класса System. После выполнения фрейм удаляется  
  }

  private static void printAll(Object o, int i, Integer ii) {  
    Integer uselessVar = 700;
// 5 Ничего  
    System.out.println(o.toString() + i + ii);
// 6 Загрузка класса System. Создание фрейма.  Создание ссылки вида String преобразованного объекта Object. Создание еще двух новых ссылок при выполнении операции "+" и удалении старых ссылок. После выполнения фрейм удаляется  
    }  
}
```
