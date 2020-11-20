# CustomLintChecksDoNotWork

Custom lint rules doesn't work in *AGP 3.5.4 / Lint 26.5.4*.
```./gradlew :mylibrary:lint``` leads to BUILD SUCCESSFUL, although there is a custom rule violation.
Check ```c8d39ba7d9d04575542352ce1322d7e1745f6fd0``` commit.

But with starting with *AGP 3.6.0 / Lint 26.6.0* ```./gradlew :mylibrary:lint``` start failing as expected.
Check ```14a52400ab37801c066c246641a0544c5b3f3fb0``` commit.
