# BasicViewBinding
This repo illustrates use of basic view binding.

# View binding
View binding is a feature that allows you to more easily write code that interacts with views. Once view binding is enabled in a module, it generates a binding class for each XML layout file present in that module. An instance of a binding class contains direct references to all views that have an ID in the corresponding layout.

## Add the following in the app's build.gradle,

```groovy
 android {
  buildFeatures {
        viewBinding true
    }
```

## And in Activity and so on,
```groovy
binding = ActivityMainBinding.inflate(layoutInflater)
        setContentView(binding.root)
       
```
