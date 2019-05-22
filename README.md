#include <iostream>
using namespace std;
class CRect{
    int w, h;
  public:
    CRect(int,int);
    int Area() {return w*h;}
};
CRect::CRect(int x, int y) {  // 생성자의 구현
  w = x;
  h = y;
}
int main () {
  CRect r(4,5);
  cout << "(4,5) Area is: " << r.Area();
  return 0;
}
