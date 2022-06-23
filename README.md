# FunFacts
FunFacts is an example of Modular architecture


![Alt Text](https://github.com/droid-lover/FunFacts/blob/master/images/FunFactsAppbySachin.jpg) 

## This Project is built using Kotlin,we will use in this App :
* Modular architecture
* Dependency Injections HILT,
* MVVM, 
* Coroutines, 
* Lottie animations, 
* Jetpack components central navigation 
* and buildSrc for central dependencies management.

### <a href="https://medium.com/native-mobile-bits/modular-android-app-architecture-build-to-scale-d6f402cbd93a/">Full explaination Article here</a>

## About the author
### <a href="https://www.youtube.com/channel/UCTjQSpx2waqXTC37AgM8qyA/"> Sachin Rajput</a>
</br></br>
   
   
   In Android development we can create these kinds of Modules for us:
1. Library Module
2. Feature Module
3. App Module
</br>
</br>


1. Library Module- It can be a third party or our own functionality developed which is kind of a utility for our main project. we can use it in multiple places in our project.
2. Feature Module- In our project, we can divide functionality or flow into small units as a separate independent feature.
3. App Module- This is our Wholesome product, it will combines all the feature modules we developed and form a single entity.
</br>
</br>


In this project, 
1. Library Module is :central module that houses API calls using Retrofit.
2. Feature Modules are :catfunfacts and :dogfunfacts
3. App Module is :app module
</br>
</br>


‘buildSrc’ ( a veronica to manage API/third party dependencies)
There is also a directory buildSrc that has all the dependencies used in our App, we can create any modules and use any third-party or Android API we can define here at one place and we can use inside all the modules it will help us maintaining similar dependencies versions throughout.

```
object Modules {
    const val central = ":central"
    const val dogfunfacts = ":dogfunfacts"
    const val catfunfacts = ":catfunfacts"
}
```

Medium Article : https://medium.com/native-mobile-bits/modular-android-app-architecture-build-to-scale-d6f402cbd93a
