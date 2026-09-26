# Intent

- Intent is a messaging object provided by Android that is used to request an action from another App Component, such as starting an Activity, starting a Service, sending a Broadcast, or communicating between application components.
- There are four types of app components:
  - Activities
  - Services
  - Broadcast receivers
  - Content providers

- For example, an Intent can be used to:
  - Open another Activity  
  - Start a Service
  - Send data from one Activity to another
  - Start another application
  - Open a web page
  - Make a phone call
    ```Java
      Intent intent = new Intent(Intent.ACTION_DIAL);
      intent.setData(Uri.parse("tel:9876543210"));
      
      startActivity(intent);
    ```
    
  - Send an email
    ```Java
      Intent intent = new Intent(Intent.ACTION_SENDTO);
      intent.setData(Uri.parse("mailto:example@gmail.com"));
      startActivity(intent);
    ```
    
  - Share text/images
  - Broadcast a message


## Types of Intent

There are two major types of Intent:

                 Intent
                   │
          ┌────────┴────────┐
          │                 │
      Explicit          Implicit
       Intent             Intent

### 1.Explicit Intent:

An **Explicit Intent** specifies exactly which component should handle the request.

Basic Syntax:-
```Java
  Intent intent = new Intent(CurrentActivity.this, TargetActivity.class);
  startActivity(intent);
```

Example:- 
```Java
      Intent intent = new Intent(this, SecondActivity.class);
      intent.putExtra("username", "Shivam saini");
      intent.putExtra("age", 22);
      intent.putExtra("isLoggedIn", true);
      intent.putExtra("salary", 15000.50);
      startActivity(intent);
```

```Java
      // SecondActivity.java
      String username = getIntent().getStringExtra("username");
      int age = getIntent().getIntExtra("age", 0);
      boolean isLoggedIn = getIntent().getBooleanExtra("isLoggedIn", false);
      double salary = getIntent().getDoubleExtra("salary", 0.0);
```

### 2. Implicit Intent

- An Implicit Intent is an Intent in which you **do not specify the exact component or application** that should handle the request.  
- Instead, you specify **what action you want to perform**, and Android finds a suitable component that can perform that action.
- For Example:-
  Suppose your application wants to open a website.  
  You don't need to know whether the user has:
  - Chrome
  - Firefox
  - Edge
  - another browser

  You can simply write:
  ```Java
    Intent intent = new Intent(Intent.ACTION_VIEW);
    intent.setData(
        Uri.parse("https://www.google.com")
    );  

    OR

    Intent intent = new Intent(
        Intent.ACTION_VIEW,
        Uri.parse("https://www.google.com")
    );
    
    startActivity(intent);
  ```

- Suppose your application needs to perform an action that another application already knows how to perform.
  For example:
  ```
    Open a website       → Browser
    Make a phone call    → Phone/Dialer
    Send email           → Email app
    Take a picture       → Camera app
    Share text           → Sharing apps
    View a location      → Maps app
  ```

  You don't have to implement all these features yourself.
  Instead, you can send an Implicit Intent.



  
