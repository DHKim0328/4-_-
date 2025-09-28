//4주차 프로그래밍
프로그램 코드

    #include<iostream> // 상속과 생성자의 관계
    using namespace std;
    
    class Parent {
    public:
        Parent() { cout << "Parent 생성자\n"; }
    };
    
    class Child : public Parent {
    public:
        Child() { cout << "Child 생성자\n"; }
    };
    
    int main() {
        Parent p1;
        Child c1;
    
        return 0;
    }
    
    //#include<iostream> // 다중상속
    //using namespace std;
    //
    //class a {
    //public:
    //    void showa() { cout << "a" << endl; }
    //};
    //
    //class b : public a {
    //public:
    //    void showb() { cout << "b" << endl; }
    //};
    //
    //class c : public a {   // 다중 상속
    //public:
    //    void showc() { cout << "c" << endl; }
    //};
    //
    //class d : public b, public c {   // 다중 상속
    //public:
    //    void showd() { cout << "c" << endl; }
    //};
    //
    //int main() {
    //    d obj;
    //    obj.showa(); // a에서 상속
    //    obj.showb(); // b에서 상속
    //    obj.showc(); // c에서 상속
    //    obj.showd(); // d 고유
    //}
    //
    //#include<iostream> // 가상 상속 || 죽음의 다이아몬드 방지
    //using namespace std;
    //class A {
    //public: 
    //    void showA() { cout << "A" << endl; }
    //};
    //
    //class B : virtual public A {
    //    void showB() { cout << "B" << endl; }
    //};
    //class C : virtual public A {
    //    void showC() { cout << "C" << endl; } 
    //};
    //    
    //class D : public B, public C { 
    //    void showD() { cout << "D" << endl; } 
    //};
    //
    //int main() {
    //    D obj;
    //    obj.showA(); //A 하나만 존재 → 모호하지 않음
    //}
