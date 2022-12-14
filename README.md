# Applitools Example: Image Tester CLI

This is the example project for the [Image Tester CLI tutorial](https://applitools.com/tutorials/quickstart/images/cli).
It shows how to start automating visual tests
with [Applitools Eyes](https://applitools.com/platform/eyes/)
using the [Image Tester](https://github.com/applitools/ImageTester) CLI tool.

This repository contains the Image Tester JAR file (version 3.1.3) along with a set of PDFs and image files for testing.
The [`files`](files/) directory provides "original" version of the PDFs and images,
while the [`files_modified`](files_modified/) directory provides visually modified versions of the same files.

To run the Image Tester CLI, you'll need:

1. An [Applitools account](https://auth.applitools.com/users/register), which you can register for free
2. The [Java Runtime Environment](https://www.oracle.com/java/technologies/downloads/) version 9 or higher

To execute Image Tester tests, set the `APPLITOOLS_API_KEY` environment variable
to your [account's API key](https://applitools.com/tutorials/guides/getting-started/registering-an-account).

Start by setting baselines using the original files by running:

```
java -jar ImageTester_3.1.3.jar -f files/ -fb "Example: Image Tester CLI"
```

Then, check for visual differences in the modified files by running:

```
java -jar ImageTester_3.1.3.jar -f files_modified/ -fb "Example: Image Tester CLI"
```

*Note:*
You can fetch the latest version of the Image Tester JAR file at
[https://github.com/applitools/ImageTester/releases/latest](https://github.com/applitools/ImageTester/releases/latest).

**For full instructions on running this project, take our
[Image Tester CLI tutorial](https://applitools.com/tutorials/quickstart/images/cli)!**