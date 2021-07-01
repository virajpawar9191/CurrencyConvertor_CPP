#include <stdlib.h>
#include <iostream>
using namespace std;

double div(float n, float m);

int main()
{
    int choice; // for gettin choice from user
    float n;    // for getting indian currency

    do
    {
        printf("\tWelcome to Currency Convertor..\n");
        printf("\n******************************************************************************************\n");

        printf("\n******************************************************************************************\n");
        printf("\n\n\tEnter the Amount in INDIAN RUPEES:\n");
        scanf("\t%f", &n);
        printf("\n\t Choices Are::\n\n");
        printf("\t1.Kuwati Dinar\n");
        printf("\t2.Bahraini Dinar\n");
        printf("\t3.Omani Rial\n");
        printf("\t4.Jordanian Dinar\n");
        printf("\t5.Pound Sterling\n");
        printf("\t6.Cayman Islands Dollar\n");
        printf("\t7.Euro\n");
        printf("\t8.Swiss France\n");
        printf("\t9.US Dollar\n");
        printf("\t10.Canadian Dollar\n");
        printf("\n\n\t**** Enter 0 to Quite****\n\n");
        printf("\n*******************************************************************************************\n");
        printf("\tEnter the choice from 1 to 10 for Conversion:\n");

        scanf("\t%d", &choice);

        // switch
        switch (choice)
        {
        case 1:
            // for Kuwati Dinar

            printf("\n\t%f Rupees = %lf Kuwati Dinar\n\n", n, div(n, 245.10));
            printf("\tAs 1 kuwati Dinar = 245.10 Rupees\n");
            break;

        case 2:
            // for Bahraini Dinar

            printf("\n\t%f Rupees = %lf Bahraini Dinar\n\n", n, div(n, 195.98));
            printf("\tAs 1 Bahraini Dinar = 195.98 Rupees\n");
            break;
        case 3:
            // for Omani Rial

            printf("\n\t%f Rupee=%lf Omani Rial\n\n", n, div(n, 192.13));
            printf("\tAs 1 Omani Rial=192.13 Rupees\n");
            break;
        case 4:
            // for Jordanian Dinar

            printf("\n\t%f Rupee=%lf Jordanian Dinar\n\n", n, div(n, 104.16));
            printf("\tAs 1 Jordanian Dinar=104.16 Rupees\n");
            break;
        case 5:
            // for Pound

            printf("\n\t%f Rupee=%lf Pound sterling\n\n", n, div(n, 102.75));
            printf("\tAs 1 Pound Sterling=102.75 Rupees\n");
            break;
        case 6:
            //for Cayman Island

            printf("\n\t%f Rupee=%lf Cayman Islands Dollar\n\n", n, div(n, 88.66));
            printf("\t 1 Cayman Islands Dollar=88.66 Rupees\n");
            break;
        case 7:
            // for Euro

            printf("\n\t%f Rupee=%lf Euro\n\n", n, div(n, 88.72));
            printf("\tAs 1 Euro=88.72 Rupees\n");
            break;
        case 8:
            //for swiss france

            printf("\n\t%f Rupee=%lf Swiss France\n\n", n, div(n, 80.89));
            printf("\tAs 1 Swiss France=80.89 Rupees\n");
            break;
        case 9:
            // for US dollar

            printf("\n\t%f Rupee=%lf US Dollar\n\n", n, div(n, 73.86));
            printf("\tAs 1 US Dollar=73.86 Rupees\n");
            break;
        case 10:
            // for Canadian Dollar
            printf("\n\t%f Rupee=%lf Canadian Dollar\n\n", n, div(n, 60.19));
            printf("\tAs 1 Canadian Dollar=60.19 Rupees\n");
            break;

        default:
            if (choice == 0)
            {
                printf("\tThank You...!");
            }
            else
            {
                printf("\tYour entered currency is not among the top ten highest valued currency\n");
                printf("\tPlease choose the currency given above\n");
            }
            break;
        }

        printf("\n******************************************************************************************\n");

    } while (choice != 0);

    return 0;
}
// Function for conversion
double div(float n, float m)
{
    double a;
    a = n / m;
    return a;
}
