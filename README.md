# work-1

#define _CRT_SECURE_NO_WARNINGS
#include <stdlib.h>
#include <stdio.h>
#define N 9

void main()
{
	int num[N], index;
	int middleInd = N / 3;
	printf("write %d numbers please\n",N);


	for (index = 0; index < N; index++)
	{
		scanf("%d", &num[index]);
	}

	//for (index=0;index;index++)
	//{ 
	//num[index] = num[index] + num[middleInd * 2];
	//num[middleInd * 2] = num[0] - num[middleInd * 2];
	//num[0] = num[0] - num[middleInd * 2];
	//}

	//num[1] = num[1] + num[middleInd * 2 + num[1]];
	//num[middleInd * 2+ num[1]] = num[1] - num[middleInd * 2 + num[1]];
	//num[1] = num[1] - num[middleInd * 2 + num[1]];
	
	//num[2] = num[2] + num[middleInd * 2 + num[2]];
	//num[middleInd * 2 + num[2]] = num[2] - num[middleInd * 2 + num[2]];
	//num[2] = num[2] - num[middleInd * 2 + num[2]];



	for (index = 0; index < N; index++)
	{
		printf("%d", num[index]);
	}
	printf("\n");


	

	for (index = 0; index < N; index++)
	{

		if (index < middleInd) 
		{

			num[index] = num[index + (N - middleInd)];
			
		}
	
		printf("%d", num[index]);

	}

	printf("\n");

	//for (index = 0; index < N; index++)
	{

		//if ((index > 0) && (index < middleInd))
		{

			//num[index] = num[index + (N - middleInd)];
		}

		//printf("%d", num[index]);
	}





		system("pause");
}
