# FancyCustomLicensePlate_Number_Generation


```
#include <string.h>

int main () {

	printf ("Hello world\n");

	char licenseplate[5];
	int sum =0;
	for (int i=4500; i< 5000; i++ ) {
	    	sprintf (licenseplate, "%d", i );
	    	//printf ( "licenseplate = %s   ", licenseplate);
		sum =0;
	    	for ( int i=0; i< strlen(licenseplate); i++ ) {
	    	    //printf ( "   Ch = %c   ", licenseplate[i]);
	    	    //printf ( "   Dec = %d  ",  licenseplate[i] - 48);
	    	    sum = sum + (licenseplate[i] - 48 );
	    	
	    	}
	        //printf ( "Total %d\n",  sum );
		if ( sum % 9 == 0 ) {
	        	printf ( " licenseplate = %s , Found %d\n",  licenseplate, sum );

		}
        }
	    

	return -1;

}
```


The output :

```

![image](https://user-images.githubusercontent.com/14288989/221527327-c48deec3-c9a1-4749-8309-eea1e4f337d4.png)
