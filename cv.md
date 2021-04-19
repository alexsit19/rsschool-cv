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

## Experience

* Project from Android Academy in process:
[https://github.com/alexsit19/MovieApp](https://github.com/alexsit19/MovieApp)

* Calculator like a Samsung App
[https://github.com/alexsit19/Calculator_java](https://github.com/alexsit19/Calculator_java)

* Puzzle-game from my childhood (LibGdx, java). I don't see analogs of this game. But my friends call it 2d rubik cube
 [https://github.com/alexsit19/RotateAndWinGame](https://github.com/alexsit19/RotateAndWinGame) : [https://www.youtube.com/watch?v=cAeiRjyP63k](https://www.youtube.com/watch?v=cAeiRjyP63k)

## Education

* Android Academy Fundamentals
* Java Cources from ITVDN (author Eugeniy Tyhonov)
* android.developers.com CodeLabs
* BSUIR (Faculty of Radioengineering and Electronics)

## English
* A1 or A2
