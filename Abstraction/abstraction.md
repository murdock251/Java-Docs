# Abstraction

**What is Abstraction?**
-> Abstraction hides **complex implementation details**,focusing only on essential features.
-> It emphasizes **what an object does, not how it does it**, through clear interfaces.


```java
package in.nsucoding.abstraction;

public abstract class Vehicle  implements Transport{
    private int noOfTires;

    public Vehicle(int noOfTires) {
        this.noOfTires = noOfTires;
    }

//    public Vehicle(){
//    }

    //making an abstract method
    public abstract void makeStartSound();

    @Override
    public void getSetGo() {
        System.out.println("going to place");
    }

    public int getNoOfTires() {
        return noOfTires;
    }

    public void setNoOfTires(int noOfTires) {
        this.noOfTires = noOfTires;
    }

    public void commute(){
        System.out.println("going...");
    }
}
```

