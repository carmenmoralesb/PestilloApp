# Pestillo 🔐

![gif](https://user-images.githubusercontent.com/22890496/193894728-43f6d3b6-065d-4f0f-9bc5-95918ef35d86.png)

You don't have to memorize all your passwords! Use this app to store all your keys and set
Password manager is an app where you can store all your credentials in a secure and organized way. All your information will securely stored inside your device.

### Future features 🎯
- [ ] Use some encryption for the data of the app, use this alongside the PIN or app lock feature.
- [ ] A password generator following some criteria and clipboard function
- [ ] Add some lock feature, like PIN or fingerprint.
- [ ] Organise the passwords: shops, work, personal, etc..
- [ ] Add password hints to the password managed in the app

### Built With 🔩
- Kotlin - Kotlin is a cross-platform, statically typed, general-purpose programming language with type inference. Kotlin is designed to interoperate fully with Java, and the JVM version of Kotlin's standard library depends on the Java Class Library.
- MVVM - Model — View — ViewModel (MVVM) is the industry-recognized software architecture pattern that overcomes all drawbacks of MVP and MVC design patterns. MVVM suggests separating the data presentation logic(Views or UI) from the core business logic part of the application. 
- Room Persistance Library - This library provides an abstraction over SQLite and makes it a lot simpler to save and fetch data from a device's database.
- Coroutines - Coroutines are used to perform two or more tasks parallely or asynchronously. They are very useful when you need to load data from cloud into your app.
- Dagger Hilt - Dagger is a fully static, compile-time dependency injection framework for both Java and Android. It is developed by the Java Core Libraries Team at Google.

### Project Structure :hammer:

    com.pestillo            # Root Package
    
    ├── data                # Contains all the adapters for recycleviews
    |   └── database        # Contains files which define an entity or table's schema in room database
        └── model           # Contains files which define an entity or table's schema in room database
        └── network 
        └── repository 
    ├── di                  # Contains files related dependency injection
    │   └── modules        
    |
    ├── domain              # Contains the model used in the app
    |   └── model
        └── usecases 
    ├── ui                  # UI/View layer
    |   ├── activities      # Contains the UI implementation of all activities and fragments
    |   ├── factories       # Contains viewmodel factories that enable us to pass repositories in viewmodel
    |   └── viewmodels      # A communication gateway between our views and models 
    |   └── view 
    └── utils                # Utility / Helper classes
