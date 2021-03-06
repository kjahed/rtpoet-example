# RTPoet Example

This is a boilerplate project demonstrating the use of the [RTPoet](https://github.com/kjahed/rtpoet) library and
its [PapyrusRT](https://github.com/kjahed/rtpoet-papyrusrt) plugin.

### Getting started

```bash
git clone https://github.com/kjahed/rtpoet-example
```

Generate a [Github Personal Access Token](https://github.com/settings/tokens/new). You only need the
**read:packages** permission.

Append the following to [gradle.properties](gradle.properties):

```bash
gpr.user=<your_github_username>
gpr.key=<your_github_token>
```

**Note:** Never push the modified [gradle.properties](gradle.properties) to Github. For security reasons, Github will
disable your access token and you will have to generate a new one.

Build!

```bash
./gradlew build
```

### Using Kotlin (Recommended)

[KotlinExample.kt](src/main/kotlin/KotlinExample.kt) demonstrates the use of RTPoet using Kotlin. Use the command below
to run the example.

```bash
./gradlew runKotlin
```

### Using Java

[JavaExample.java](src/main/java/JavaExample.java) demonstrates the use of RTPoet using Java. Use the command below to
run the example.

```bash
./gradlew runJava
```

### References

- Refer to the [RTPoet](https://github.com/kjahed/rtpoet) repository for details regarding the
  generic [RTModel data structure](https://github.com/kjahed/rtpoet/tree/master/src/main/kotlin/ca/jahed/rtpoet/rtmodel)
  for UML-RT models. The repository also implements helpers
  to [copy](https://github.com/kjahed/rtpoet/blob/master/src/main/kotlin/ca/jahed/rtpoet/utils/RTDeepCopier.kt),
  [equate and diff](https://github.com/kjahed/rtpoet/blob/master/src/main/kotlin/ca/jahed/rtpoet/utils/RTEqualityHelper.kt)
  ,
  and [validate](https://github.com/kjahed/rtpoet/blob/master/src/main/kotlin/ca/jahed/rtpoet/utils/RTModelValidator.kt)
  RTModels.


- Refer to [RTPoet's Papyrus-RT plugin](https://github.com/kjahed/rtpoet-papyrusrt) repository for Papyrus-RT specific
  operations such
  as [reading](https://github.com/kjahed/rtpoet-papyrusrt/blob/master/src/main/kotlin/ca/jahed/rtpoet/papyrusrt/PapyrusRTReader.kt)
  and [writing](https://github.com/kjahed/rtpoet-papyrusrt/blob/master/src/main/kotlin/ca/jahed/rtpoet/papyrusrt/PapyrusRTWriter.kt)
  Papyrus-RT models,
  Papyrus-RT [primitive types](https://github.com/kjahed/rtpoet-papyrusrt/tree/master/src/main/kotlin/ca/jahed/rtpoet/papyrusrt/rts/primitivetype)
  , and RTS
  specific [protocols](https://github.com/kjahed/rtpoet-papyrusrt/tree/master/src/main/kotlin/ca/jahed/rtpoet/papyrusrt/rts/protocols)
  and
  [classes](https://github.com/kjahed/rtpoet-papyrusrt/tree/master/src/main/kotlin/ca/jahed/rtpoet/papyrusrt/rts/classes)
  .