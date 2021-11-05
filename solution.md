# To build and start the Server ##

In my case I use the gradle interface that provides the IntelliJ IDEA, but this is only a shortcut that invoke

build = `./gradlew :server:build` and bootrun = `./gradlew :server:bootRun`.

# To build and start the Client ##
First of all we have to build and boot the server before the client, and then as in the previous case

build = `./gradlew :server:build` and bootrun = `./gradlew :server:bootRun`.

## Modification added to the Server.kt ##
I changed the TODO() with:
```
                                    TranslationResponse().apply {
                                          translation="!Traduceme !"    
                                    }
```
## Result ##

    > Task :client:bootRun
    Result of translating [Translate me!] is [!Traduceme !]