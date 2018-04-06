# getArea
#include <iostream>
#include <iomanip>
using namespace std;

//function prototypes
double getLength();
double getWidth();
double getArea(double, double);
void displayData(double, double, double);

int main() 
{
	double rectangleLength = getLength();
	double rectangleWidth = getWidth();
	double rectangleArea = getArea(rectangleLength,rectangleWidth);
	displayData(rectangleLength,rectangleWidth,rectangleArea);
	system("pause");
	return 0;
}
double getLength()
{
	double length;
	cout<<"Enter the length: ";
	cin>>length;
	return length;
}
double getWidth()
{
	double width;
	cout<<"Enter the width: ";
	cin>>width;
	return width;
}
double getArea(double rectangleLength,double rectangleWidth)
{
	double area = (rectangleWidth*rectangleLength);
	return area;
}
void displayData(double rectangleWidth,double rectangleLength,double rectangleArea)
{
	cout<<"\nRectangle Data\n";
	cout<<"--------------"<<endl;
	cout<<"Length: "<<setw(3)<<rectangleLength<<endl;
	cout<<"Width: "<<setw(4)<<rectangleWidth<<endl;
	cout<<"Area: "<<setw(5)<<rectangleArea<<endl;
}
