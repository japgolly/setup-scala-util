# `setup-scala-util` GitHub Action

A GitHub Action to add Scala utilities to the PATH.

Utilities
=========

* `sbt++field` - Start sbt with the Scala version described by an sbt build field.

  ```sh
  > grep -h 'val scala.*=' project/*.scala
      val scala2          = "2.13.6"
      val scala3          = "3.0.2"

  > sbt++field scala2 test
  # Runs sbt ++2.13.6 test
  ```

* `sbt-const` - Extract the string literal from a `val` or `def` field in your sbt build.

  Example:

  ```sh
  > grep -h 'val scala.*=' project/*.scala
      val scala2          = "2.13.6"
      val scala3          = "3.0.2"

  > sbt-const scala2
  2.13.6
  ```
