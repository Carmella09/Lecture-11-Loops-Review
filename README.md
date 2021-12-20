# Lecture-11-Codes

//LOOPS

Execute this code and see what’s the issue

    #include <iostream>
    #include <string>
    using namespace std;
    int main()
    {
      int y;
      cout << "Enter a number you want the table of: " << endl;
      cin >> y;

      while (cin.fail())
      {
        cout << "Invalid command enter the number again: " << endl;
        cin.clear();
        cin.ignore(1000, '\n');
        cin >> y;
      }
      for (int x = 0; x <= 10; x++)
      {
        cout << y << " x " << x << " = " << y * x << endl;
      }
    }
    
Write the code in while loop to give this output (Descending Stars, Seven Lines)

    #include<iostream>
    using namespace std;
    int main()
    {
      int x = 1, y = 1;
      while (x <= 5)
      {
        y = x;
        while (y <= 5)
        {
          cout << "*";
          y++;
        }
        x++;
        cout << endl;
      }
    }

Write the code in while loop to give this output (Rising Stars, Five Lines)

    #include<iostream>
    using namespace std;
    int main()
    {
      int i = 1, j = 1;
      while (i <= 5)
      {
        j = 1;
        while (j <= i)
        {
          cout << "*";
          j++;
        }

        i++;
        cout << endl;
      }
    }

Write the code in while loop to give this output (Rising and Falling Stars) 

    #include<iostream>
    using namespace std;
    int main()
    {
      int x = 1, y = 1; 
      while (x <= 5)
      {
        y = x;
        while (y <= 5)
        {
          cout << "*";
          y++;
        }
        x++;
        cout << endl;
      }

      int i = 1, j = 1;
      while (i <= 5) 
      {
        j = 1; 
        while (j <= i)
        {
          cout << "*";
          j++;
        }

        i++;
        cout << endl;
      }
    }
    
Factorial

    #include <iostream>
    using namespace std;
    int main()
    {
        cout << "Enter a number: " << endl;
        double n, factorial = 1;
        cin >> n;
        for (int i = n; i > 0; i--)
        {
            factorial = i * factorial;
        }
        cout << "The factorial of " << n << " is: " << factorial << endl;
    }


Exercise : For Loop - Table

    #include <iostream>
    using namespace std;
    int main()
    {
        int n, p;
        cout << "Enter a number: ";
        cin >> n;
        while (cin.fail())
        {
            cout << "Invalid Input" << endl;
            cout << "Enter the number again: ";
            cin.clear();
            cin.ignore(1000, '\n');
            cin >> n;
        }
        for (int i = 0; i <= 10; i++)
        {
            p = n * i;
            cout << n << " i " << i << " = " << p << endl;
        }
    }


Exercise : Convert the previous code into while loop - Table

    #include <iostream>
    using namespace std;
    int main()
    {
        int n, p, i = 0;
        cout << "Enter a number for multiplication tabele: ";
        cin >> n;

        while (cin.fail())
        {
            cout << "Invalid Input" << endl;
            cout << "Enter the number again: ";
            cin.clear();
            cin.ignore(1000, '\n');
            cin >> n;
        }
        while (i <= 10)
        {
            p = n * i;
            cout << n << " i " << i << " = " << p << endl;
            i++;
        }
    }


Exercise : For Loop - Table

    #include <iostream>
    using namespace std;
    int main()
    {
        int n, n2, p;
        cout << "Enter a number for multiplication table: ";
        cin >> n;

        while (cin.fail())
        {
            cout << "Invalid Input" << endl;
            cout << "Enter the number again: ";
            cin.clear();
            cin.ignore(1000, '\n');
            cin >> n;
        }
        cout << "Enetr the number in which it ends (up to 10 only): ";
        cin >> n2;

        while (cin.fail())
        {
            cout << "Invalid Input" << endl;
            cout << "Enter the number again: ";
            cin.clear();
            cin.ignore(1000, '\n');
            cin >> n2;
        }

        for (int i = 0; i <= 10; i++)
        {
            p = n * i;
            cout << n << " x " << i << " = " << p << endl;
        }
    }

Exercise : Do-While Loop - Find the 9s

    #include <iostream>
    using namespace std;
    int main()
    {
        int n = 100, s = 0;
        do
        {
            if (n % 9 == 0)
            {
                cout << "Number: " << n << endl;
                s = s + n;
            }
            n++;
        } while (n <= 200);
        cout << "\nSum: " << s << endl;
    }

