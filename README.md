#include <stdio.h>
#include <string.h>

int main()
{
	label :
		printf("\ntype :   (a) km   - mile\n\t (b) inch - foot\n\t (c) cm   - inch ");

	char typ;
	printf("\n\nenter word :");
	scanf("%c", &typ);
	double num;

	if (typ == 'a'){
		printf("\n enter km : ");
		scanf("%lf", &num);
		printf("%lf km = %lf mile\n\n\n",num, (num / 1.609344));}
		
	else if (typ == 'b'){
		printf("\n enter inch  : ");
		scanf("%lf", &num);
		printf("%lf inch = %lf foot\n\n\n",num, (num / 12));}
		
	else if (typ == 'c'){
		printf("\n enter cm  : ");
		scanf("%lf", &num);
		printf("%lf cm = %lf inch\n\n\n",num, (num / 2.54));}
		
	else{
		goto label;
		}
		
	char qut[20] ;
	scanf("%s",&qut);
	if(strcmp(qut,"exit")==0){
		printf("\t\t\t - EXIT -");
		break
	}
	else{
		continue ;
	}
	

	return 0;
}
