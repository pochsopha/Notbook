### Java
#### main class
```js

package inheritance_class.phone;

public class Inheritance_ClassPhone {

    public static void main(String[] args) {
Class_iphone dc = new Class_iphone (200,"IME","Model", "Color");
        dc.showdata();
    }
    
}
        
```
#### Class phone
```js
//Inheritance....................
package inheritance_class.phone;


public class Classphone {
  float price;
    String IME,Model,Color;
    public Classphone(){
    }

    public Classphone(float price, String IME, String Model, String Color) {
        this.price = price;
        this.IME = IME;
        this.Model = Model;
        this.Color = Color;
    }

    
public void showdata()
{
    System.out.println("price           :"+price);
    System.out.println("IME      :"+IME);
    System.out.println("Model   : "+Model);
     System.out.println("Color  : "+Color);
    
}
}  
    



```
### class_iphone
```js
package inheritance_class.phone;


public class Class_iphone extends Classphone {

    float price;

    public Class_iphone() {
    }

    public Class_iphone( float price, String IME, String Model, String Color) {
        super(price, IME, Model, Color);
        this.price = price;

    }

    public void showData() {
        super.showdata();
        System.out.println("price:" + price);
    }

}
```
