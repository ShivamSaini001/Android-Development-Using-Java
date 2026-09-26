# Intent

- Intent is a messaging object provided by Android that is used to request an action from another App Component, such as starting an Activity, starting a Service, sending a Broadcast, or communicating between application components.
- There are four types of app components:
  - Activities
  - Services
  - Broadcast receivers
  - Content providers

- For example, an Intent can be used to:
  - Open another Activity
    ```Java
      Intent intent = new Intent(this, SecondActivity.class);
      startActivity(intent);
    ```
    
  - Start a Service
  - Send data from one Activity to another
    ```Java
      Intent intent = new Intent(this, SecondActivity.class);
      intent.putExtra("username", "Shivam saini");
      startActivity(intent);
    ```

    ```Java
      // SecondActivity.java
      String username = getIntent().getStringExtra("username");
    ```

  - Start another application
  - Open a web page
    ```Java
      Intent intent = new Intent(
              Intent.ACTION_VIEW,
              Uri.parse("https://www.google.com")
      );
      
      startActivity(intent);
    ```
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

### 2. Implicit Intent

An Implicit Intent does not specify a particular component.
Instead, it specifies the **action that needs to be performed**.



