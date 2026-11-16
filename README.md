# rep11
11주차 과제
```
#define _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
#include <string.h>
void main(void) {
	char str[1000], r[1000];
	printf("문장 입력: ");
	scanf("%[^\n]", str); // 엔터(\n) 전까지 공백 포함 문장 전체 입력
	// 문자열 끝에서부터 거꾸로 한 글자씩 출력
	for (int i = (int)strlen(str) - 1; i >= 0; i--)
		r[i] = str[i];
	r[strlen(str)] = NULL;
	printf("%s", r);
}
```
