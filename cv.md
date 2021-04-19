#  Aliaksandr Situshkin
## Contacts
* email: alexsit12@gmail.com
* mobile: +375 (29) 686-47-90 (viber)
* telegram: @alexsit12

## Summary
My goal to get a job android developer.
It amazing when I can run written by me app on own mobile device. And I can got some user experiens from other people. And I can understand how people use my app and I can  do it more better.

## Skils
* Programming language: Java, Kotlin
* Architecture: MVP, MVVM
* Android Studio
* Basic knowledge in Android (Activity, Fragments, RecyclerView ets.)
* Understanding OOP Principles
* Git

## Code Example
```kotlin
class FragmentMoviesListViewModel(private val movieListInteractor: MovieListInteractor): ViewModel() {

    private val mutableLiveData = MutableLiveData<List<Movie>>()
    val liveData: LiveData<List<Movie>> = mutableLiveData

    private fun loadData() {
        viewModelScope.launch {
            try {
                mutableLiveData.value = movieListInteractor.getMovies()
                } catch (e: Exception) {
                Log.d("DEBUG exception", "${e.message}")
            }
        }
    }

    fun getData(): LiveData<List<Movie>> {
        loadData()
        return liveData
    }
}
```
