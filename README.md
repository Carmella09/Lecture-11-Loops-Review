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

version (1)

    #include <iostream>
    using namespace std;
    int main()
    {
        int i = 0, j = 0, n = 5;
        while (i < n)
        {
            while (j <= i)
            {
                cout << "*";
                j++;
            }
            j = 0;
            i++;
            cout << endl;
        }
    }
    
version (2)

    #include<iostream>
    using namespace std;
    int main()
    {
      int i = 0;
      while (i < 5){
        i++;
        int j = 1;
        while (j <= i){
          j++;
          cout << "*";
        }
        cout << endl;
      }
    }
  
version (3)

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



Exercise : For Loop



Exercise : Convert the previous code into while loop



Exercise : For Loop


Exercise : Do-While Loop

Find the 9s
