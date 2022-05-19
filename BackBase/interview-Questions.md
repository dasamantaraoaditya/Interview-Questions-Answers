# Back-Base

## Core-Java
- Different examples on method overriding 
```
class Parent {
    public void display(){
        System.out.println("Parent Method");
    }
}

class Child extends  Parent{
    public void display() --check this-- throws IOException, throws RunTimeException, no exception handled {
        System.out.println("Child Method");
    }
}

class App {
    public static void main(String[] args) {
        Parent p = new Child();
        p.display();
    }
}
1.do we get runtime exceptions compile time etc ...
```

```
class Parent {
    public void display(Object o)  {
        System.out.println("Object Method Called");
    }
    public void display(String s)  {
        System.out.println("String Method Called");
    }
}

class App {
    public static void main(String[] args) {
        Parent p = new Parent();
        p.display(null);
    }
}
```
- Access modifiers and overriding method
```
class Parent {
    public int display(String s)  {
        try{
            System.out.println("try");
            return 10;
        }catch(Exception e){
            System.out.println("catch");
            return 20;
        }finally {
            System.out.println("finally");
            return 30;
        }
    }

}
class App {
    public static void main(String[] args) {
        Parent p = new Parent();
        System.out.println(p.display(null));
    }
}
```
- Data Structures
  - Hashmaps implementation
  - hashSet implementations
```
public class Employee {
    private int id;
    private String name;
    public Employee(int id, String name){
        this.id = id;
        this.name = name;
    }
    @Override
    public int hashCode() {
        return id;
    }
}
class App {
    public static void main(String[] args) {
        Set<Employee> dataSet = new HashSet<>();
        dataSet.add(new Employee(1, "Backbase"));
        dataSet.add(new Employee(1, "Backbase"));
        System.out.println(dataSet.size());
    }
}
```

- Object Equals and hashcode uses with examples
  - What is the Contract between equals method and hashcode ?

- Multithreading
  - synchronization
  - Thread safe means and how to achive it 
- Searialization

## Spring 
- Difference between @component and @bean
- Accessing spring beans 
- Bean scopes
- What is @lookup

## Hibernate
- Best practives in hibernate
- Can you tell something about the N+1 SELECT problem in Hibernate?
- cascading
- @Transactional

## Unit testing 
- doReturn and thenReturn difference

## Problem Solving 
### WAP count occurence of each char in a String ?

Input: javaBBb
Output: j=1, a=2, v=1, b=1, B=2
```
int[] freq = new int[26];

Map<Character,Integer> map = new HashMap<>();

for(int i =0;i<str.length();i++)
{
if(map.containsKey(str.charAt(i)){
map.put(str.charAt(i),map.get(str.charAt)+1);
}
else{
map.put(str.charAt(i),1);
}
}
```

### Remove Duplicates from Array ?

Input: arr :  [1,2,3,4,3,4,5,2,3,1}
Output: [1,2,3,4,5]
```
List<Integer> list = Arrays.asList(arr);

List<Integer> ans = list.stream().filter((a,b)->a!=b).collect(Collecters.asList());
```
