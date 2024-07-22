## Исходный код программы. Ошибки закоменнтированы.
#include <iostream>
using namespace std;

/*struct point {
	double m_x;
	double m_y;
	point(double x, double y) {
		m_x = x;
		y = y;// некорректная инициализация переменной y
	}
} // отсуствие точки с запятой

void print_point(const point& point_object) {
	std::cout << "x:" << point_object.m_x << ", y: "
		<< point_object.m_y << std::endl;
}

int Main()// название функции main() должно начинаться с строчной буквы
{
	int i;
	for (i = 0; i < 5; i++); { // лишний символ ; после условия цикла
		point my_point(i, 2 * i);
		print_point(my_point);
	}
	return 0;
}
------------------------------------------------------------------------------
## Исправленный код:
struct point
{
	double m_x;
	double m_y;
	point(double x, double y)
	{
		m_x = x;
		m_y = y;
	}
};

void print_point(const point& point_object) {
	std::cout << "x:" << point_object.m_x << ", y: "
		<< point_object.m_y << std::endl;
}

int main()
{
	int i;
	for ( i = 0; i < 5; i++) {
		point my_point(i, 2 * i);
		print_point(my_point);
	}
	return 0;
}