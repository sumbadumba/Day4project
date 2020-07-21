# Day4project

/*숙제 -- > 가진 돈 수치로 코인 환산해서 출력 만들기
		가진 조개 껍데기 2,864,953,217개
		1 동화  100껍대기(100)
		1 은화 = 200동화(20000)
		1 금화 = 120 은화(2400000)
		1 루비 = 80 금화(192,000,000)
*/

//14루비
#include <stdio.h>
#define Shellfish = 2864953217;//이 많은 숫자들은 뭐지..

void changeMn(int r, int g, int s, int b);

int main()
{
	int ruby = 192000000;
	int gold = 2400000;
	int silver = 20000;
	int bronzes = 100;

	changeMn(ruby, gold, silver, bronzes);

}
void changeMn(int r, int g, int s, int b)
{
	__int64 a = 2864953217;
	int value = 0;
	int change = 0;

	printf("환산을 하면 \n\n");

	value = a / r;
	printf("%d루비 ", value);
	change = a % r;

	value = change / g;
	printf("%d골드 ", value);
	change = change % g;

	value = change / s;
	printf("%d은화 ", value);
	change = change % s;

	value = change / b;
	printf("%d동화 ", value);
	change = change % b;

	printf("%d조개 껍데기입니다. \n\n", change);

}

#include "stdafx.h"
//
//#define MAX_LEVEL 99
//
//
//int global = 20;//전역변수
//int value1 = 10;
//
//int index = 0;
//void Recursive()//void 형들은 return이 있으면 return에서 끝난다.(재귀함수 = 함수에서 함수를 호출)(위험요소 : 끝나는 return 값이 꼭 있어야한다)
//{//(끝나는 값이 없으면 터진다)
//	printf("Recursive : %d\n", index++);
//
//	if (index > 10)
//		return;
//	Recursive();//함수안에서 본인함수를 부를 수 있다.
//
//}
//
//int main()
//{
	/*Recursive();
*/
	//int value1 = 20;
	//printf("\n\n\n\t %d", ::value1);// ::  = 범위 지정자(전역변수의 값을 가져온다)(안쓸경우 지역변수의 값을 가져온다)

	/*rintf("%d\n", MAX_LEVEL);
	*/



	//int i = 1;
	//i += MAX_LEVEL;
	//printf("%d\n", i);

	//const int temp6 = 20;//const = 지정자(constant의 약자) 지속적인...

	//temp6 = 10;const에는 할당이 안된다 == define과 같음



//}


// #include <stdio.h>
//★함수★
//
//void Function();//밑에 함수내용을 적으면 함수의 정의를 안해도 되는데 밑에
//함수 선언		//있으면 정의를 해야함.
//int Function2()//반환형 
//{
//	int returnValue = 10;
//	int returnValue2 = 20;
//
//	return returnValue + returnValue2;//반환값
//
//}
//void Function3(int value1, int value2, float value3)//int value1에 parameta로 준다(인자)로 전달한다.
//{
//	printf("value1 = %d\n", value1);
//	printf("value2 = %d\n", value2); 
//	printf("value3 = %.2f\n", value3);
//
//
//}
//int main()//메인함수
//{
//	int a = 10;
//	int b = 20;
//	float c = 30.0f;
//
//	//Function();
//	int result = Function2();
//	printf("result = %d", result);
//
//	Function3(a, b, c);//30을 쓸 때 명시적으로는 int형이다.(float)권고사항 
//	//다만 반대로 인트를 써야할곳에 소숫점을 쓰면 소수는 날라간다.
//}
//
//void Function()
//{
//	printf("Function i called!");
//}
//
//국영수 점수를 인자로 받아 평균을 반환하는 함수를 만들어서 Main 함수에서 호출하라
//
//#include<stdio.h>
//int average(int m, int e, int k)
//{
//	float aver = 0;
//
//	aver = (m + e + k) / 3;
//
//	return aver;
//}
//int gkorean = 80;//전역변수에서 쓴 변수와 같은 수를 쓰면 컴퓨터는 헷갈려한다.(g를 붙여서 전역변수인것을 표시한다)
//
//int main()
//{
//	int math = 0; //지역변수라고 한다.
//	int english = 0;
//	int korean = 0;
//	float value = 0;
//
//	printf("당신의 수학 점수는?");
//	scanf("%d", &math);
//
//	printf("당신의 영어 점수는?");
//	scanf("%d", &english);
//
//	printf("당신의 국어 점수는? ");
//	scanf("%d", &korean);
//
//	value = average(math, english, korean);
//
//	printf("당신의 평균점수는 %.1f입니다.", value);
//}
//
//int Average(int korean, int english, int math)//센세의 코드))))))))))))))))
//{
//	int average = (korean + english + math) / 3;
//
//	return average;
//
//}
//
//int main()
//{
//	int k = 80;
//	int e = 69;
//	int m = 39;
//
//	int average = Average(k, e, m);
//
//	printf("average = %d", average);
//
//}
//
//실습2 
//애완 동물 종류를 입력받아 출력하는 함수를 만드세요.
//- scanf 나 cin을 통해
//- 입력된 값은 강아지는 1, 고양이는 2, 그외 반려동물 3, 없으면 0;
//- main()함수에서 만든함수를 호출
// 만든 함수 내부에서 printf나 cout으로 출력
// 출력 형식 "당신의 반려동물은 xxx이군요. "
//
//#include<stdio.h>
//
//void A()
//{
//	printf("A Called!");
//}
//void B()
//{
//	printf("B Called!");
//}
//void C()
//{
//	printf("C Called!");
//}
//
//void youranimal(int animal)
//{
//	if (animal == 1)
//	{
//		printf("당신의 반려동물은 강아지 이군요.");
//	}
//	else if (animal == 2)
//	{
//		printf("당신의 반려동물은 고양이 이군요.");
//	}
//	else if (animal == 3)
//	{
//		printf("당신의 반려동물은 그 밖이군요.");
//	}
//	else
//	{
//		printf("당신은 반려동물이 없군요.");
//	}
//}
//
//int main()
//{
//	int which_animal = 0;
//
//	printf("당신이 반려동물은 어떤 종류인가요? 1.강아지, 2.고양이, 3.나머지, 4.없음");
//	scanf("%d", &which_animal);
//	scanf_s("%d", &which_animal, sizeof(which_animal)); 정확한 크기를 알 수 있어서 안전하게 쓸 수 있다.
//
//
//	youranimal(which_animal);
//
//	A();
//	B();
//}
//#include<stdio.h>
//void A()
//{
//	printf("a called!");
//}
//void B()
//{
//	printf("b called!");
//}
//void C()
//{
//	printf("c called!");
//}
//
//int main()
//{
//	A();
//	B();
//}
//
//int main()
//{
//	int petType;
//
//	switch (petType)
//	{
//	case 1:
//		break;
//	case 2:
//		break;
//	case 3:
//		break;
//
//	default://switch문에는 default를 꼭 넣어야함에 주의
//		break;
//
//	}
//}

//숙제 1
// 서기 년도를 단기 년도로 계산해서 출력하는 함수 만들기
// 예) 서기 1988 = > 단기 4321
// 인자로 서기 년도를 int 형을것
// 함수 내부에서 단기 몇년인지 출력
// main() 함수에서 scanf나 cin으로 서기년도를 입력


//숙제 2
//  2개의 숫자를 입력받아서 '*'문자를 이용해 직사각형을
//  그리는 함수를 만들기
//  가로 :첫번째 문자
//	세로: 두번째 문자
//	함수 내부에서 사용자로부터 입력을 받을것
// * 숫자는 1~10까지만 유요하도록 할 것
// 직사각형의 내부는 가득차 있지 않아도 인정
