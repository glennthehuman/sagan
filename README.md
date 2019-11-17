## Sagan: the spring.io site and reference application

Welcome! The code in the master branch of this repository is deployed and running right now at [spring.io](http://spring.io). The [blog][], the collection of [guides][], and everything else you see there is implemented right here.

In addition to the practical purpose of powering Spring's home on the web, this project is designed to serve as a *reference application*--a resource that developers can use to see how the [Spring team][] have used Spring to implement a real-world app with a few interesting requirements. We hope you'll find it useful!

## Getting started

You'll find everything you need to get started in the [project wiki][], but you can also begin by simply browsing through the repository and finding what's of interest to you. You'll find README files in key directories, and Javadoc throughout the code. The app and all of its documentation are designed with the idea of a 'self-guided tour' in mind.

#### Build

[For Windows 10] Start Powershell as Administrator.

From within the root directory of your repository, the following command will build both the Sagan site and indexer applications, running all unit and integration tests along the way:

> _**Tip:** New to Gradle? Check out [[Gradle tips]]!_

    ./gradlew build

Or, on Windows:

    gradlew.bat build


When the build is finished, you should see the following:
```
BUILD SUCCESSFUL
```

### Next steps

You're now ready to [[import into IDEA or Eclipse]] or you can [[run the site locally]] straight away.

(See [project wiki][] for other details.)

#### Run the site locally from the command line

[For Windows 10] Start Powershell as Administrator.

From the root directory of your sagan repository, run the following:

> _**Tip:** New to Gradle? Check out [[Gradle tips]]!_

```
./gradlew :sagan-site:bootRun
```

After a few seconds, you should see:
```
sagan.SiteApplication : Started SiteApplication
```

Now, go to <http://localhost:8080> and you should see homepage. Click around and explore a bit—you should find the site is identical in every way to what you see at [spring.io](http://spring.io).

> _**Note:** The exceptions to the above are rendering guides and blogs and also search. Out of the gate, you'll get 500 errors when you try to perform a search, the guides will be empty and blogs will also fail to compile. To remedy this, you'll need to [[enable search locally]] and [[run the renderer service]]._


### Next steps

At this point, you may want to [[build everything]] or [[import into IDEA or Eclipse]] if you have not already.

(See [project wiki][] for other details.)

## Q&A and issue tracking

If you have any questions, feedback, or feature requests, don't hesitate to [add an issue][].

## Contributing

[Pull requests](https://help.github.com/en/desktop/contributing-to-projects/creating-a-pull-request) are welcome; see the [contributor guidelines](CONTRIBUTING.md) for details.

## License

Sagan is released under the [BSD-3 license](LICENSE.md).


[blog]: https://spring.io/blog
[guides]: https://spring.io/guides
[Spring team]: https://spring.io/team
[project wiki]: https://github.com/spring-io/sagan/wiki
[add an issue]: https://github.com/spring-io/sagan/issues
