Infinite View Pager
===============

A [simple] circular View Pager for Android


### Gradle build

To use the library in your project add the following to your `build.gradle` :
<pre>
dependencies {
    // another dependencies ...
    implementation 'com.android.support:<b>appcompat-v7:27.1.0</b>'
    <b>implementation 'id.bungamungil:infinite-view-pager:1.0.1'</b>
    // another dependencies ...
}
</pre>


### Notes from Original Author

- Wrapped scrolling should now be possible with your `ViewPager`. The pages you see are not duplicates - each page from your `PagerAdapter` is only created once and then reused. This means you do not have to worry about managing multiple instances of the same `Fragment`.

- It is only possible to achieve wrapping when you have at least 4 pages. This is because of the way the `ViewPager` creates, destroys, and displays the pages. No fix for the general case has been found.