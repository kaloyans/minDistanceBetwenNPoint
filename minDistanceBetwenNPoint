#include<stdio.h>                                                                                                                                                                           #include<stdlib.h>#include<math.h>
#define MAX_COORDINATES 1000 
structdot { 
	int number;
	double x;
	double y;
};
structdistanceInfo { 
	doubledistance;
	int dot1;
	int dot2;
};
intmain()
{
	int n;
	dot *dots; 
	do {
		printf("Enterthedotsnumber: ");
		scanf_s("%d", &n);
	} while (n < 1); 
	printf("\n");
	dots= (dot*)malloc(n*sizeof(dot)); 
	if (!dots) { 
		printf("Cannotlocatememoryfordots\n");
		exit(1);
	}
for (int i = 0; i < n; i++) {
		dots[i].number = i; 
		dots[i].x = rand() % MAX_COORDINATES; 
		dots[i].y = rand() % MAX_COORDINATES; 
	}
doublebuff; 
	distanceInfominDistance;
	minDistance.distance = sqrt((pow(dots[1].x - dots[0].x, 2)) + (pow(dots[1].y - dots[0].y, 2)));
	minDistance.dot1 = dots[0].number;
	minDistance.dot2 = dots[1].number;

	for (int i = 0; i < n; i++) {
		for (int j = i + 1; j < n; j++) {
			buff = sqrt((pow(dots[j].x - dots[i].x, 2)) + (pow(dots[j].y - dots[i].y, 2)));
			if(buff<minDistance.distance) { 
				minDistance.distance = buff;
				minDistance.dot1 = dots[i].number;
				minDistance.dot2 = dots[j].number;
}
		}
	}
	printf("Thesmallestdistanceis %lf\nItisbetweendot %d anddot %d.\n", minDistance.distance, minDistance.dot1, minDistance.dot2);
		system("pause");
	return 0;
}
