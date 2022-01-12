# uit1
#include <iostream>
using namespace std;
struct Point {
	double x, y;
};
void Nhap(Point *&a){
	a = new Point; //cap phat
	cin >> a -> x >> a -> y;

}
Point *Nhap(){
	Point *a;
	a = new Point;
	cin >> a->x >> a->y;
	return a;
}
void Xuat(Point *&a){
	cout << "("<< a->x << ", " << a->y << ")";
}
int main() {
    Point *A , *B;
    Nhap(A);
    B = Nhap();
    Xuat(A);
    std::cout << " and ";
    Xuat(B);
    return 0;
}
